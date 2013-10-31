vision
======

A place to discuss and track product vision for the Hypothes.is software ecosystem.

Roadmap
=======

[X] Means done!

### Unified DB release Done
- [X] Unify live and reserved username db

### Candidate release (0.0.6) - Done, Jan 9, 2013
- [X] Flash messages (#233)
- [X] Static asset build script (#161)
- [X] Finish registration form flow (#159)
- [X] Separate detail and bucket views (#162)
- [X] slide over ([issue](https://github.com/hypothesis/h/issues/150), [mockup, click off of sidebar and then back onto summary view to see](http://jtremback.github.com/fakebarDos/build-cea4d78/index.html))
- [X] Drag / resize sidebar frame (Done 11/25/2012)
- [X] replies
- [X] Markdown (Done 11/15/2012)

### Extension release (0.1) - CURRENT / IN DEVELOPMENT
- [X] Chrome extension ([issue](https://github.com/hypothesis/h/issues/43), [wiki](Browser-extension))
- [X] UI polish (streams, standalone)
- [X] Annotations should show up in sidebar when launched if available ([issue #464](https://github.com/hypothesis/h/issues/464)) (done w/ multi-frame)
- [X] Improve documentation
- [X] Personal annotations ([wiki](visibility), [mockup- click on "reply" control in annotation and then "public" dropdown in upper right corner](http://jtremback.github.com/fakebarDos/build-cea4d78/index.html) This mockup depicts a superset of the behavior. For this release, it will not have the group selection)
- [X] Delete and modify / edit annotations ([issue](https://github.com/hypothesis/h/issues/213), [wiki](Deletion-and-Editing), [mockups](http://jtremback.github.com/fakebarDos/build-82150b4/index.html))
- [X] Link to an annotation ([wiki](Linking-to-an-annotation), [mockup of standalone annotation](http://jtremback.github.com/standalone/build-a8213d8/index.html), [mockup of source site in frame](http://jtremback.github.com/hypotheFrame/build-7881d1e/index.html))
- [X] Fuzzy Anchoring ([wiki](fuzzy-anchoring))
- [X] New alpha page
- [X] User streams
- [X] Kill slide-over ([issue #466](https://github.com/hypothesis/h/issues/466))
- [X] Improve Auth/login/Reg process
- [X] Fix broken navigation arrows ([issue #435](https://github.com/hypothesis/h/issues/435))
- [X] Delete private annotation bug “Sorry something went wrong with the annotation store”.  ([issue #472](https://github.com/hypothesis/h/issues/472))
- [X] Expose all features in annotation menu (reply/edit/delete) if space available. ([issue #476](https://github.com/hypothesis/h/issues/476))
- [X] Edit button should say “Save” not “Edit” ([issue #478](https://github.com/hypothesis/h/issues/478))
- [X] Two annotation bug ([issue #328](https://github.com/hypothesis/h/issues/328))


### MVP release (target: Sep 1, 2013)
- [X] Simple new user tour / help tips ([issue #469](https://github.com/hypothesis/h/issues/469))
- [X] [Basic Tagging](https://docs.google.com/document/d/1hdoxJZMxf2MCwT5IwuHvrkJ3s9qXCvtJx6oEP4QB5IE/edit?usp=sharing) ([issue #514](https://github.com/hypothesis/h/issues/514))
- [X] [Control Bar](https://docs.google.com/document/d/1meXJaS1OdkrvC4-veCE4w5o9O9pP0tHO-7PsIzHTCt0/edit?usp=sharing) (done in alpha)
- [X] [Always-on Annotations (all annotation highlighted on source page)](https://docs.google.com/document/d/12dqspVLnvrLSBt0-YchjsEPt7F_84C5VeT3cMh7ebjM/edit?usp=sharing)  ([issue #531](https://github.com/hypothesis/h/issues/531)) _requested by law-group_
- [X] [Search / Filters](https://docs.google.com/document/d/1mLxjZWAd-G35_DagYv9RcpMBoXUnoXBSQjZh8eodbJQ/edit?usp=sharing) ([issue #549](https://github.com/hypothesis/h/issues/549))
- [X] [Highlighting Mode for researchers v1](https://docs.google.com/document/d/1QSKY_Lc5et4F0pwu0d4AttxIME_E4rjaCHzuwQIgiyc/edit?usp=sharing) ([issue #530](https://github.com/hypothesis/h/issues/530))
- [X] [Unattached/unanchored annotations](https://docs.google.com/document/d/1KG6AoTPzI4_r3K996ggqR18qi_jdoogBjLpU9ytDEjQ/edit?usp=sharing) ([issue #115](https://github.com/hypothesis/h/issues/115))
- [X] [Notifications of new annotations](https://docs.google.com/a/hypothes.is/document/d/1gD38gLJB7uxf2NZDqbuxUF1gRzHpqLhxkqNf5IVn8As) - click to load (simplified version of realtime updating) ([issue #568](https://github.com/hypothesis/h/issues/568))
- [ ] Appify the website (login, register, etc)
- [ ] Architecture / infrastructure work
    - [ ] Interframe communication
        - [ ] Being able to target an iFrame for use with [Epub.js](https://github.com/fchasen/epub.js) and others.
        - [ ] Listening mode ([issue 43](https://github.com/hypothesis/h/issues/43))
        - [ ] Enable turning off h. from page action icon ([issue 468](https://github.com/hypothesis/h/issues/468))
    - [X] Unit/functional testing

### Post MVP Features
- [X] Wordpress Plugin ([early but fully functional version](http://wordpress.org/plugins/hypothesis/))
- [ ] Architecture / infrastructure work
    - [ ] Better test coverage
    - [ ] Exception handling (rollbar, source maps, etc) (issues [#347](https://github.com/hypothesis/h/issues/347) and [#393](https://github.com/hypothesis/h/issues/393))
    - [ ] Auth out of the sidebar see the app.net hackathon branch.
- [ ] PDF support ([wiki](PDF), [issue #758](https://github.com/hypothesis/h/issues/758))
    - [ ] FF extension ([issue #43](https://github.com/hypothesis/h/issues/43), [wiki](Browser-extension))
- [ ] Image annotation ([issue #380](https://github.com/hypothesis/h/issues/380))
- [X] Streams + Search ([issue #719](https://github.com/hypothesis/h/issues/719))
- [ ] Simple anti-spam controls ([hover over anyone but woah2, click downward arrow for flag menu](http://jtremback.github.com/fakebarDos/build-82150b4/index.html)) _requested by law group_
- [ ] Groups (issues: [#120](https://github.com/hypothesis/h/issues/120), [#121](https://github.com/hypothesis/h/issues/120), [#495](https://github.com/hypothesis/h/issues/495); [specs](https://docs.google.com/document/d/17HDaujAt5P9o5x2Yinr8jL_tZS_3Zd36VBYbpPz-bkM/edit?usp=sharing))   _requested 3x by law group_
    - [ ] Link-only annotation view ([issue #424](https://github.com/hypothesis/h/issues/424))
    - [ ] Social views ([issue #535](https://github.com/hypothesis/h/issues/535), [specs](https://docs.google.com/document/d/1bXRjm7rL8xlwsb-kXiRfxSeB8qLShSzmG1MP6cB7JI8/edit?usp=sharing))
- [ ] Views and sorts ([issue #640](https://github.com/hypothesis/h/issues/640))
- [ ] Realtime updating ([issue #209](https://github.com/hypothesis/h/issues/209))
- [ ] Alerts / notifications (via email-- replies, follows, new annotations, stored searches, etc.) ([issue 
#581](https://github.com/hypothesis/h/issues/581))
- [ ] Direct linking V2 ([issue #769](https://github.com/hypothesis/h/issues/769), [specs](https://docs.google.com/a/hypothes.is/document/d/1x9e7jX3Xor6kMpU0cqD0wV8Om8Mxa2VEvH3zGBPLx3c/edit)) (Peter Bol req, req by law group & unanimously req'd by journalists)
- [ ] Upvote / downvote moderation & meta-moderation ([wiki](Matching-Metamoderators)) ([needs work](http://jtremback.github.com/actStreamMock/build-1327dbf/index.html))
- [ ] Highlight mode v1.5 (color separation for highlights vs annotations) ([issue #622](https://github.com/hypothesis/h/issues/622), [specs](https://docs.google.com/document/d/1QSKY_Lc5et4F0pwu0d4AttxIME_E4rjaCHzuwQIgiyc/edit), [further discussion](https://docs.google.com/document/d/1kRVMVI1Pt2YdlDMfT3WESxa3rL7YqZj0xsHHG23GhHU/edit))
- [ ] Account functions (Change email address, delete account, profile info) (issues [#551](https://github.com/hypothesis/h/issues/551), [#632](https://github.com/hypothesis/h/issues/632))
- [ ] Export annotations to HTML, text, csv, json? (issues [#394](https://github.com/hypothesis/h/issues/394) and [#490](https://github.com/hypothesis/h/issues/490))
- [ ] Math support ([issue #720](https://github.com/hypothesis/h/issues/720))
- [ ] Print-friendly mode for streams ([issue #716](https://github.com/hypothesis/h/issues/716))
- [ ] Following & other social features ([issue #131](https://github.com/hypothesis/h/issues/131) and possibly others)
    - [ ] "Humble" or Follower-only visibility mode ([issue #536](https://github.com/hypothesis/h/issues/536))
- [ ] Favoriting (hover any annotation and click on the star icon to favorite the annotation) ([issue #119](https://github.com/hypothesis/h/issues/119), [mockup](http://jtremback.github.com/fakebarDos/build-82150b4/index.html))
- [X] User documentation ([issue #680](https://github.com/hypothesis/h/issues/680))
- [ ] Login with Twitter and Oauth
- [ ] Feedback system ([PR #759](https://github.com/hypothesis/h/pull/759))
- [ ] Settings panel (issues [#551](https://github.com/hypothesis/h/issues/551) and [#552](https://github.com/hypothesis/h/issues/552))
    - [ ] User profiles ([issue #128](https://github.com/hypothesis/h/issues/128))
- [ ] RSS for streams ([issue #391](https://github.com/hypothesis/h/issues/391))
- [ ] Style 404 page ([issue #480](https://github.com/hypothesis/h/issues/480))
- [ ] Embedded annotations ([issue #141](https://github.com/hypothesis/h/issues/141); [early version](http://hypothes.is/blog/embedded-annotations)) _use case for H2O_
- [ ] Tagging V2: reference external ontologies ([issue #142](https://github.com/hypothesis/h/issues/142), [specs](https://docs.google.com/document/d/1hdoxJZMxf2MCwT5IwuHvrkJ3s9qXCvtJx6oEP4QB5IE/edit))
- [ ] Author identification.
- [ ] Hypothes.is Flavored Markdown (Clickable @username, #tag and $annotationid links in annotations, going to the right place.) ([issue #763](https://github.com/hypothesis/h/issues/763))
- [ ] Annotating w/ images ([issue #600](https://github.com/hypothesis/h/issues/600))
- [ ] Hypothesis.js packaging
- [ ] Hightlighting Mode V2 Support for an Amazon Kindle like Popular Highlights ([issue #622](https://github.com/hypothesis/h/issues/622), [specs](https://docs.google.com/document/d/1QSKY_Lc5et4F0pwu0d4AttxIME_E4rjaCHzuwQIgiyc/edit), [further discussion](https://docs.google.com/document/d/1kRVMVI1Pt2YdlDMfT3WESxa3rL7YqZj0xsHHG23GhHU/edit))
- [ ] Quotation autocomplete
- [ ] Readers packed w/ extension (pdf.js, epub.js, readium.js) ([issue #512](https://github.com/hypothesis/h/issues/512) about PDF.js))
- [ ] Wiki-style annotations / Collaborative authorship ([issue #300](https://github.com/hypothesis/h/issues/300))
- [ ] Experiment w/ sticky-note style UI in certain circumstances? ([issue #341](https://github.com/hypothesis/h/issues/341))
- [ ] Heatmap vs. Document Map option.
- [ ] Allow the ability to scroll the sidebar and have it navigate the page.
- [ ] “Click for more” - collapsing replies above or below a certain point to focus in a particular area.
- [ ] Lock sidebar out (“pin” it).  Squeeze DOM.  This could be located in the Control Bar. ([issue #491](https://github.com/hypothesis/h/issues/491))
- [ ] Logging out in one tab doesn’t log out of all tabs. ([issue #475](https://github.com/hypothesis/h/issues/475))
- [ ] Offline annotations
- [ ] Selectable store of annotations in extension
- [ ] Collapsing threads ([issue](https://github.com/hypothesis/h/issues/188), [mockup, scroll to see](http://jtremback.github.com/fakebarUno/build-e7f7897/index.html))
- [ ] Review markup to ensure accessibility via screenreaders, etc.
- [ ] Increased text size support for reduced vision
- [ ] Annotations of annotations ([issue #64](https://github.com/hypothesis/h/issues/64)) _noted by law group_
- [ ] WYSIWYG editor ([discourse](https://github.com/discourse/discourse/blob/master/app/assets/javascripts/external/Markdown.Editor.js))
- [ ] Annotations that suggest changes to the source
- [ ] Features targeting mobile functionality (issues [#237](https://github.com/hypothesis/h/issues/237), [#238](https://github.com/hypothesis/h/issues/238), [#587](https://github.com/hypothesis/h/issues/587), [#588](https://github.com/hypothesis/h/issues/588))
- [ ] Integrate w/ the Internet Archive to archive a web page anytime it's annotated. _req by Perma project_
- [ ] Architecture / infrastructure work
    - [ ] Change implementation of notifications (issues [#734](https://github.com/hypothesis/h/issues/734) and [#726](https://github.com/hypothesis/h/issues/726))
    - [ ] Use conneg for REST API Versioning (for smooth upgrades) (issue [#733](https://github.com/hypothesis/h/issues/733))
    - [ ] Search in annotation body using the rendered form, not the source (issue [#677](https://github.com/hypothesis/h/issues/677))
- [ ] Provide alternate methods for selecting text ([issue #382](https://github.com/hypothesis/h/issues/382)) _requested by @IanMulvany of PeerJ_
- [ ] Social: Sharing via twitter, facebook ([issue #122](https://github.com/hypothesis/h/issues/122))
- [ ] Identity: Login with Mozilla persona (issues [#126](https://github.com/hypothesis/h/issues/126), [#348](https://github.com/hypothesis/h/issues/348))
- [ ] Client-side encryption ([issue #344](https://github.com/hypothesis/h/issues/344))
- [ ] Keyboard shortcuts ([issue #722](https://github.com/hypothesis/h/issues/722)) _requested by [@aculich](https://github.com/aculich)_
- [ ] V2 of always-on annotations ([issue #620](https://github.com/hypothesis/h/issues/620))
- [ ] Always-on mode redesign: show only stuff in currently selected view ([issue #639](https://github.com/hypothesis/h/issues/639))
- [ ] Messaging: ability to send another user a private message ([issue #136](https://github.com/hypothesis/h/issues/136))
- [ ] Chat interface in sidebar for whatever page you're on ([issue #147](https://github.com/hypothesis/h/issues/147))
- [ ] Importing annotations ([issue #768](https://github.com/hypothesis/h/issues/768))
- [ ] manually insert document equivalences into our DB ([issue #765](https://github.com/hypothesis/h/issues/765))
- [ ] Narratives / Threads / Trails ([issue #385](https://github.com/hypothesis/h/issues/385)) _requested by @IanMulvany of PeerJ_
- [ ] Web of ideas ([issue #386](https://github.com/hypothesis/h/issues/386))
- [ ] Reconstructing existing articles as Narratives ([issue #767](https://github.com/hypothesis/h/issues/767))
- [ ] Ability to handle dynamic content (issues [#397](https://github.com/hypothesis/h/issues/397) and [#744](https://github.com/hypothesis/h/issues/744))
- [ ] Separation of the discourse of the subject matter from speech acts ([issue #667](https://github.com/hypothesis/h/issues/667))
- [ ] entity-context annotations ([issue #766](https://github.com/hypothesis/h/issues/766]))
- [ ] Faster loading (async scan) (issues [#334](https://github.com/hypothesis/h/issues/334), [#335](https://github.com/hypothesis/h/issues/335) and [#710](https://github.com/hypothesis/h/issues/710))
- [ ] Support for IE (10+) ([issue #585](https://github.com/hypothesis/h/issues/585))
