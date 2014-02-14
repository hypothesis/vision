At the time of writing (January 2014), hypothesis/h is using the observer branch of hypothesis/annotator, which diverged from okfn/annotator some time ago. Additionally, hypothesis/h embeds okfn/annotator-store but is currently diverged (though less so than annotator) primarily for some basic model and index changes.

This document is meant to provide an overview of the components and develop a plan to move both forward and toward convergence (defined by greater code-sharing, with enhancements and fixes rapidly made available to the community).

# Summary of incompatibilities

## annotator
Hypothes.is has diverged for primarily two reasons.

 - hypothesis/annotator
  - uses .target with OA-like designations instead of .text/.quote properties
  - in latest work, changes to where selection is handled
  - strategy delegation for anchoring
 - okn/annotator
  - is likely more or less bw-compatible
  - has changed little in annotator.coffee since the original fork
  - has made some change toward preferring ._local for presentational/view data

### reconciliation plan
There is support for adopting an Open Annotation model in the Annotator (citation needed). The Hypothes.is fork has transitioned to a use of targets as Objects but has not yet adopted the same for bodies. Doing so would replace the current .tag and .text fields. Some demonstration of these typed bodies needs to be made.

A possibility exists to formalize application interfaces which might simply abstract away the difficulties posed by a diversity of annotation serializations. If these core aspects of an annotation (provenance, target, body) can be interposed through hooks or getter/setter methods then integrators can be given the ability to plug their own model in. The attractiveness of this approach is compounded by the possibility of integrators providing a model factory to the annotator framework during configuration which streamlines integration with their chosen application framework, making annotation a natural citizen of a web application.

Some work has already been done to place some patterns for extending annotator. There are some further possible advancements that should probably be made:

 - The addition of a helper in base classes in the spirit of Backbone's .extend
  - clarifies integration for non-coffee users
  - encourages decomposition of core actor methods into useful hooks
   - Examples include store serialization, authentication of requests, anchoring passes

The addition of `._local` in the (unreleased) annotator 2.0 suggests that an indirection might ease some integrations. If the annotation model interface implement hooks for Annotator components to act over, control over the separation between stored and presentational state can be left to the application developer. Persistence may be transparently provided by the user-provided Annotation implementation. Such would be the case if an angular `$resource` or `Backbone.Collection` were presented with adapters as the annotation storage. In this way, the functionality currently provided by plugins like `Annotator.Plugin.Store` might be subsumed by frameworks already in use by application developers. The solution is to give them control of the model which Annotator components interrogate and react to. Such a design would also make providing an Annotator-1.2.x-compatible storage wrapper while defaulting Annotator-2.0 to a model which designates explicit, typed body and target relations for an annotation.

The master branch at okfn/annotator should be largely compatible with existing deployments, unless customization has been extensive as it has with hypothesis/annotator. The existing annotation life-cycle events have been preserved, but the API of Annotator objects has changed. This is largely cosmetic, and the CRUD methods could be reintroduced.
*** @csillag: I do not know enough about how your current evolution of anchoring as plugin interacts with Annotator events. Could you add some detail?***

With a pluggable model providing a migration strategy for clear body/target separation, Annotator 2.0 could be ready for release pretty quickly. We should decide whether we wish to try to contribute the anchoring strategies at this moment, or defer to an Annotator 2.1 release. That work will involve merging the changes to the core Annotator class to support pluggable selectors and document access strategies.

The work to unify hypothesis and annotator is then largely a matter of driving consensus on the appropriate interface between framework authors and custom support for *selection* and *selectors*:

  [This section needs writing]

## annotator-store
hypothesis/annotator-store and okfn/annotator-store differ only in the settings on the ElasticSearch index. These changes accommodate slightly different interpretations of deletion, tag normalization, and the difference posed by the use of targets and selectors.

### reconciliation plan

 - Support migrations
  - Basic tooling/example migration. KISS.
  - Maybe multi-index support in ES helpers
  - Model hooks for app configuration (`g.Annotation`, perhaps)
