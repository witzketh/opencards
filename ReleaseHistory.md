﻿The release history of OpenCards.

## OpenCards 2.5.1 (5.1.2017)

* Added [openfx package dependency](http://stackoverflow.com/questions/34243982/why-is-javafx-is-not-included-in-openjdk-8-on-ubuntu-wily-15-10) for Ubuntu/Debian


## OpenCards 2.5 (1.5.2016)
* Markdown Integration Improvements

## OpenCards 2.4 (11.4.2016)
* Preserve aspect ratio when rendering slides
* Support for markdown files as flashcard sets (section titles are questions, section content are answers)
* Improved rendering of Cards (using POI v3.14)


## OpenCards 2.3 (18.9.2017)
* Added Dutch translation (thanks to  Rutger Scholtens)
* Improved german translation
* Fixed links to help
* Improved Rendering of Cards (using POI v3.12)

## OpenCards 2.2 (22.2.2012)
* Added Simplified Chinese translation (thanks to Lee Darren)
* Added Japanese translation (thanks to Eberhard Herzog)
* More smooth (=antialiased) slide rendering on windows and linux
* Fixed issue 24: Incorrect rendering of text-shape bounding boxes
* Stability improvements based on community feedback

## OpenCards 2.1 (1.11.2011)
* fixed inocorrect email-addrees for automatic bug-reporting
* Improved synchronization with ppt-files
* Added drag-and-drop support for ppt-files into OpenCards
* Improved integration of last-minute learning
* Better visualization of new cards in schedule preview
* Open current slide during learning in PowerPoint by double-clicking it


## OpenCards 2.0.0 (30.9.2011)
- update notfication when version of OpenCards are released (issue 19)
- example card sets in category model to flatten learning curve for new OC-users (issue 22)


## OpenCards 2b3 (29.9.2011)
* CSV-Importer (issue 1)
* fixed many rough edges in the macos integration
* proper windwos executable
* finished porting of all major v1.5 functionality

## OpenCards 2b2 (26.9.2011)
* Changed from OpenOffice plugin to standalone application that uses PowerPoint files as major file-format
* Most other features (categorization, scheduler, ltm-learning) have been ported
* Temporarily removed features: Reversed cards-sides



------------------------------------------------------------------------------------------------------
OpenCards4Impress release history (no longer developed or maintained)

## OpenCards 1.5.1 (2.9.2009)
* Fixed problem when removing last card-set from category

## OpenCards 1.5 (aka OpenCards 2 beta1, 20.5.2009)
* increased minimal system requirements to java6 and OpenOffice3.0
* tag arbitrary shapes as questions
* automatic parsing of directory structures into a the category model sub-tree
* category deletions now require additional user confirmation
* Streamlined problem reporting by auto-composing report email
* sortable columns in LTM-Manager
* dramatically improved stability on slow systems (and especially with OpenOffice 3.1, which is much less snappy compared to 3.0)
* persistent divider-locations for LTM-Manager


## OpenCards 1.0.1 (19.1.2008)
* new: notification about exceeded maximal new items limitation
* improved: replaced logging monitor with log-file
* fixed: OC crashes on missing question mode
* fixed: OC crashes when XStyle-name is null
* improved: introduced short delay before hiding slide-pane to avoid occasional crashes


## OpenCards 1.0 (25.9.2008)
* fixed: crash when remove title when there's no title
* fixed: slide sorter hiding does not work in OpenOffice3
* improved: OpenOffice3 integration
* dev: updated build.xml to OpenOffice3-package structure


## OpenCards 0.16.3  (aka OpenCards 1.0 RC 6) (23.9.2008)
* fixed: Keyboard shortcuts are broken when recently found items are being processed
* fixed: Drag'n'Drop seems to be broken quite often
* removed: Untranslated dialog that appeared after the end of each last-minute learning session
* More verbose error messages in crash dialog


## OpenCards 0.16.2  (aka OpenCards 1.0 RC 5) (8.9.2008)
* Adaptive learning dialog layout depending on height/width-ratio
* Custom field delimiters when importing flashcards (feature request 2054529)
* Bulgarian translation (thx to Stefan Stefanov)
* fixed: Stability problems when switching from one scheduled card-file to the next one
* fixed: session skipping is broken


## OpenCards 0.16.1  (aka OpenCards 1.0 RC 4) (11.8.2008)
* fixed: OC crashes after preferences have been reseted (bug 2037976 )
* fixed: Preferences dialog could be more compact (bug 2039120 )
* fixed: OC crashes if last slide is deleted during learning presentation when this slide is shown in question mode


## OpenCards 0.16  (aka OpenCards 1.0 RC 3) (23.7.2008)
* Automatic guessing of character encoding when importing flashcards from csv-files
* Started OpenCards manual. It's implemented in docbook to allow an easy compilation into pdf, html, java help or ooo-help
* New learning mode: When CTRL is hold while a new learning session is started in the LTM-Manager OC will include all new items. This overrides the default behavior which just incrementally includes new items into the learning process. Refer to the manual for details.
* CTRL+C opens configuration dialog for the current slide when being in a learning session
* fixed: Refreshing mode included new (unseen) items
* fixed: new item counts in table do not match panel-counts
* fixed: Warning on Impress shutdown is shown more than once


## OpenCards 0.15.2  (aka OpenCards 1.0 RC 2) (27.6.2008)
* fixed: oc crashes on double-ESC (bug 1997180)


## OpenCards 0.15.1 (aka OpenCards 1.0 RC 1) (15.6.2008)
* Added (optional and by default inactive) logging monitor that should ease to issue-reporting. This monitor can be activated under Preferences->Advanced
* improved in-session file-transitions (which should also increase stability)
* fixed: OC hangs forever occassionally when startingW/terminating learning sessions


## OpenCards 0.15 (29.5.2008)
* Automatic hiding of the slide sorter pane during learning (feature request 1890815)
* Added Italian translation (thx to Silvio Gavagnin)
* Added Greek translation (thx to Akis Vassiliadis)
* Added Portuguese translation (thx to Ricardo Umpierre)
* fixed: OC-toolbar-icons don't look too nice (bug 1915621)
* cosmetics: Toolbar is now named "OpenCards" now and not anymore "Add-on 1"


## OpenCards 0.14 (28.4.2008)
* GZip compression of serialized flascard-data
- smaller files (~25%)
- 100x faster (no joke!): much faster loading of presentations containing open cards-data (for 600 cards Spanish.odp loadtime was
  reduced from 85.6s to 0.35s, ltm-manager startup for 50 card-files down from 15s to ~1s)
  - As a drawback OC is not backwards compatible to prior releases
* New much more smooth dialog-handling while loading next flashcard-file in ltm-mode
* OC User-ID which allows to detect imported card-sets automatically (feature request 1944488)
* OC proposes to learn items detected during learning immediately (feature request 1939956)
* Added French translation (thx to Xavier Domont)
* Added Spanish translation (thx to Fernando Ossandón)
* Simplified and improved many many UI-strings
* New preferences implementation for Linux when Java6 is used ( hacked around http://bugs.sun.com/bugdatabase/view_bug.do?bug_id=6519088 )
* Simplified UI: Removed 'Flatten' from category-context menu because nobody understood its meaning
* improved: Preferences-dialog chooses an optimal size automatically
* improved: open import-FAQ in browser if import has failed completely
* fixed: import-file not closed after import
* fixed: the file-chooser on "add card-file" does not appear


## OpenCards 0.13 (24.3.2008)
* New logo for OpenCards (bug 1791943)
* Much better long-term scheduling algorithm (bug 1912235)
* Learning success is now visualized instead of 'number of repetitions' (which was buggy anyway) in ltm-manager
* Forced refreshment of flashcards (feature requests 1907526, 1880284)
* Current slide becomes recentered in Impress if 'Home' is pressed or the learn-progress-bar is double-clicked (feature request 1922573)
* improved: Up-key can be used now to skip the current item (feature request 1908938)
* improved: F1 now opens the help in the browser
* improved: made tooltips of feedback-buttons more newbie-friendly
* improved: Don't attempt to change the L&F on Linux (which should fix the missing OC-menu in Ubuntu)
* fixed: Import of UTF-16 files fails (bug 1910386)
* fixed: OpenCards crashes if all but one item in the last-minute learning were skipped
* fixed: scheduling broken after midnight (bug 1908379)

## OpenCards 0.12.1 (24.2.2008)
* fixed: Auto-Discovery dead-lock
* improved: AboutDialog updated to 2008

## OpenCards 0.12. (22.2.2008)
* Integrated OpenCards into context-menu of Impress slide-pane which allows to configure single flashcards (feature request 1895484)
* Monitoring of flashcard-directories: Auto-discovery of uncategorized flashcard-files (feature request 1896374)
* Customizable flashcard-retention, which is used to scale the spacing intervals between scheduled reviews
* Customizable locations for the Category-tree-file (feature request 1888114)
* improved: New color-scheme for last-minute cardbox-view which highights the current flashcard (bug 1876302)
* improved: Session-persistent random-reverse-states for ltm-learning (bug 1875864)
* improved: Cardfile settings dialog is now fully localized
* fixed: There is a probability >0 that flashcards within a file obtain the same OpenCardsID
* fixed: OpenCards is blocked after LastMinute-Learning was started once using the file-context menu in the LTM-Manager
* improved: use more fields of OOo extension framework (publisher, release notes, display name)

## OpenCards 0.11.3 (26.1.2008)
* fixed: links to help-page and contribution-page are broken

## OpenCards 0.11.2 (20.1.2008)
* fixed: cards which were scheduled for tomorrow yesterday are scheduled for tomorrow also today

## OpenCards 0.11.1 (14.1.2008)
* urgent bugfixes

## OpenCards 0.11 (13.1.2008)
* Added icons to context-menu of file-view in the Long-Term memorization manager
* Added link to the OpenCards-flashcard repository to the OpenCards-menu
* LTM-Manager becomes invisible if a card-file is double-clicked
* The preferences-dialog is resizeable now (which should fix the dialog-layout for ubuntu)
* fixed:  Auto-select user-interface language
* fixed: negative scheduling-dates in tooltip
* fixed: two-keys-feedback
* fixed: the result of a forced syun-operation is not serialized


## OpenCards 0.10 (21.12.2007)
* Insession Ultra-Short-Time Rescheduling
* Statistics-panel are updated on selection-changes in the file-table
* New menu-structure
* Added possibility  to remove all OpenCards-related data from the current presentation
* Support for three sided cards (needs to be enabled in Preferences->Advanced)
* New selectable synchronization-policies
1) explicit sync (with progress-bar) before starting LongTermMemorization-learning (forced sync)
2) silently synchronize card-files which need to be opened anyway because they contain items scheduled for today (lazy sync)
* Optional (Preferences->"Show Feedback-Tooltips") tooltips for LTM-feedback-buttons which predict the the next scheduled date
* Improved: LongTermMemorization-Manager instance is reused for all open OpenOffice-frames
* Overhauled settings dialog
1) New tab for general settings
2) Improved layout of the dialog; moved some preferences to more appropriate categories
* Configurable behavior when skipping flashcards during learning (defer in session, defer to next session, defer to tomorrow)
* Changed learn-dialog to allow skipping of cards also if the complete card is shown (the "cancel learning" button was dropped, to cancel a learning session the system-close button (cross) needs to be used)
* Invitation dialog for translators
* Added warning/explanation dialog when no entitled slides are contained in the current presentation
* Flashcard-printing manager which temporarily duplicates all slides to contain on the duplicated slide the question/keyword of each slide only


## OpenCards 0.9.3 (6.12.2007)
* fixed: scheduling dates in LTM-Manager are not updated correctly

## OpenCards 0.9.2 (5.12.2007)
* fixed: context-menu for categories and cardfiles does not appear under linux

## OpenCards 0.9.1 (5.12.2007)
* fixed: category-tree serialization failed under linux and winXP

## OpenCards 0.9 (4.12.2007)
* First beta of OpenCards :-)
* Auto-synchronization on changes, insertions and deletions of slides while being in learning mode
* Streamlined keyboard control interface by using arrow-keys only
* Common drag'n'drop operations for LTM-Manager
* Optional automatic recursing into child-categories in LTM-Manager
* Schedule files based on mean "learn-urgency"
* Major performance improvements
* Fixed: negative scheduling times in LTM-Manager
* Fixed: invalid configuration of windows in dual-screen setups
* Fixed: STM* and LTM-learning can be started within a single Impress-frame in parallel
* Various minor stability and usability improvements

## OpenCards 0.8.1

* urgent bugfixes
* fixed: start learning in empty ltm-manager failed
* fixed: wrong intial box in leitner system

## OpenCards 0.8

* Import of flashcards from csv-files
* Simplified long-term learning manager
* Improved overall stability, by taking more care of OpenOffice-events
* Improved long-term learning algorithm
* Automatic detection of changes in card-sets
* New UI for LastMinute-Learning
* Started wiki on website which allows to share own card-sets with other users
* Unified API of different learning apporoaches
* Bug-fixes

## OpenCards 0.7

* new artwork
* flashcard-category management
* new longterm memorization scheduling mechanism
* improved last-minute learning
* improved locale-detection (use oo-locale instead of document-locale)
* improved odp-serialization (use custom document properties instead of custom user properties)
* four flashcards modes (normal, reverse, random reverse, both sides independent) (major feature!)
* improved presentation of flashcards
* bug-fixes
* fully compatible with OpenOffice 2.3


## OpenCards 0.6

* keyboard mapping for learn-dialog
* settings management
* configurable leitner system
* i18n (German, Portugese, English, French)
* card-side reversing
* removed Java6 dependencies
* integrated versioning and autoupdate-information into oxt-file
* bug report dialog in case of exceptions
* presentation dependent learn-settings

## OpenCards 0.5

* Leitner flashcard learning
* Different learning strategies
* Implemented as OpenOffice extension
* Persistent session states
* OpenSource: Published under BSD-license