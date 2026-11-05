# Documentation Audit – OpenStreetMap Wiki

This document summarizes the problems we found in the original OpenStreetMap documentation before rewriting it.

**Detailed audits** for each topic, with "before" screenshots, are in the comments of each topic's **GitHub issue** on our Project board. This page gives a summary of each original page and the key findings across all pages.

## Quality framework

We evaluated every original page against the eleven-point quality framework described in our proposal.

| # | Criterion | Question we asked |
|---|---|---|
| 1 | Helpful | Does the page help the reader reach their goal? |
| 2 | Comprehensive | Does it include all the information and steps the reader needs? |
| 3 | Searchable | Can the reader easily find the page and the information within it? |
| 4 | Visual | Are there clear, current screenshots or diagrams where they help? |
| 5 | Usable | Is it organized so readers can follow it easily, with topic types (concept, task, reference) kept separate? |
| 6 | Readable | Are sentences short and clear, and is the text easy to scan? |
| 7 | Reliable | Is the information accurate and up to date with the current OSM website? |
| 8 | Grammatically correct | Is it free of spelling, grammar, and punctuation errors? |
| 9 | Translatable | Is it free of idioms, unexplained jargon, and text inside images? |
| 10 | Accessible | Do images have alt text, are headings used correctly, and are links descriptive? |
| 11 | Appropriate tone | Is the tone suitable for the audience (friendly, clear, professional)? |

## Summary by original page

| Original page | Our topics (issue) | Key problems | Criteria most affected | Audited by |
|---|---|---|---|---|
| [About OpenStreetMap](https://wiki.openstreetmap.org/wiki/About_OpenStreetMap) | What is OpenStreetMap? (#11) | Serves several audiences at once, so none gets enough depth; no images; unexplained jargon (slippy map, API, Overpass, planet file); link lists instead of explanations | Helpful, Visual, Translatable | Ashna Ayaz |
| [Browsing](https://wiki.openstreetmap.org/wiki/Browsing) | Available Map Layers (#12), How to Find a Place on the Map (#13), How to Switch Map Layers (#14), How to Share a Map Link (#15) | Tasks, concepts, and reference mixed together; missing steps (searching, switching layers); layers listed without descriptions; relies on numbered callouts, some of which conflict; technical URL details in general-user content; jargon (Nominatim, Mapnik) | Usable, Comprehensive, Visual, Readable | Ashna Ayaz |
| [Notes](https://wiki.openstreetmap.org/wiki/Notes) | What Are Map Notes? (#16), Map Note Markers and Statuses (#17), How to View Notes on the Map (#18), How to Comment on a Note (#19), How to Add a Note to the Map (#20) | Concept, task and reference content are mixed on one page, and the title "Notes" does not say what the page is about; no short definition or life cycle of a note; marker and status information is buried in a task section and split across two sections, and the marker table is incomplete; steps are written in paragraphs and are spread across the page; the last step is missing for adding a note; commenting on a note is explained in one sentence with no steps; login advice is contradictory; screenshots are small and unexplained, and marker images have no alt text | Usable, Comprehensive, Helpful, Visual, Readable, Searchable, Accessible | Macwilliam Appianing |
| [Beginners Guide 1.3](https://wiki.openstreetmap.org/wiki/Beginners_Guide_1.3) | [OSM Data Elements: Nodes, Ways and Relations (Issue #21)](https://github.com/AshnaAyaz/Copy-Editors-Crusade/issues/21) · [Improved Wiki](https://github.com/AshnaAyaz/Copy-Editors-Crusade/wiki/OSM-Data-Elements%3A-Nodes%2C-Ways-and-Relations); [How to Add a Missing Place (Issue #24)](https://github.com/AshnaAyaz/Copy-Editors-Crusade/issues/24) · [Improved Wiki](https://github.com/AshnaAyaz/Copy-Editors-Crusade/wiki/How-to-Add-a-Missing-Place) | The explanation of OSM data elements is buried in a broader editing guide, with limited diagrams and practical examples. The page mixes concept and reference content but provides no step-by-step instructions for adding a place, no iD screenshots, and an outdated editor reference. | Helpful, Searchable, Usable, Readable, Visual, Reliable | Kadria Hussein |
| [Glossary](https://wiki.openstreetmap.org/wiki/Glossary) | [OSM Glossary for Beginners (Issue #22)](https://github.com/AshnaAyaz/Copy-Editors-Crusade/issues/22) · [Improved Wiki](https://github.com/AshnaAyaz/Copy-Editors-Crusade/wiki/OSM-Glossary-for-Beginners) | Beginner terms are mixed with numerous technical, organizational, and historical terms. Some key definitions are too abstract, while common beginner terms such as "point of interest" and "upload" are missing. | Helpful, Usable, Readable, Comprehensive | Kadria Hussein |
| [OpenStreetMap account](https://wiki.openstreetmap.org/wiki/OpenStreetMap_account) | [How to Create an OSM Account (Issue #23)](https://github.com/AshnaAyaz/Copy-Editors-Crusade/issues/23) · [Improved Wiki](https://github.com/AshnaAyaz/Copy-Editors-Crusade/wiki/How-to-Create-an-OSM-Account) | Registration instructions no longer fully match the current sign-up interface. The procedure is written in paragraphs without a current form screenshot and is embedded among several unrelated account-management topics. | Reliable, Usable, Helpful, Searchable, Readable, Visual | Kadria Hussein |
| [iD](https://wiki.openstreetmap.org/wiki/ID) | [How to Edit an Existing Place (Issue #25)](https://github.com/AshnaAyaz/Copy-Editors-Crusade/issues/25) · [Improved Wiki](https://github.com/AshnaAyaz/Copy-Editors-Crusade/wiki/How-to-Edit-an-Existing-Place) | The page describes the editor and its technical background but does not explain how to modify an existing place. Its only editor screenshot dates from 2013 and lacks a descriptive caption and alt text. | Helpful, Usable, Readable, Visual, Accessible, Reliable | Kadria Hussein |
| [Map features](https://wiki.openstreetmap.org/wiki/Map_features) | Tags and Map Features (#26), Common Map Feature Tags (#27), How to Add Tags to a Feature (#28) | | | Anna Ovsiannikova |
| [Buildings](https://wiki.openstreetmap.org/wiki/Buildings) | How to Draw a Building (#29) | | | Anna Ovsiannikova |
| [Addresses](https://wiki.openstreetmap.org/wiki/Addresses) | How to Add an Address (#30) | | | Anna Ovsiannikova |
| [Pick your mapping technique](https://wiki.openstreetmap.org/wiki/Pick_your_mapping_technique) | Armchair vs Outdoor Mapping (#31) | Existing page is a hodgepodge of introductory information, developer insights, irrelevant or useless images, and an abundance of technical information that has little to do with the topic | Reliable, Usable, Visual  | Luigi Benetton |
| [iD/Shortcuts](https://wiki.openstreetmap.org/wiki/ID/Shortcuts) | iD Keyboard Shortcuts (#32) | The page admits up front that the keyboard shortcuts are both part of another software company's tools that are integrated into OSM AND that people found them out partly by trial and error. There are also blatant errors on this page (the Mac does not have an F15 key). The author placed the keyboard shortcuts BEFORE the explanations of the features they trigger, which is a mistake on a page written in English. This reference list also includes instructions on how to use features that are triggered by keyboard shortcuts—such information ought to be on another page. | Helpful, Searchable, Usable | Luigi Benetton |
| [Beginners Guide 1.4.2](https://wiki.openstreetmap.org/wiki/Beginners_Guide_1.4.2) | How to Upload Your Changes (#33) | The wiki page describes itself as a "stub" and asks for help completing it. The actual tasks are not actually on this page even though the page title promises to explain "Uploading your changes to OSM." | Comprehensive, Usable, Helpful | Luigi Benetton |
| [Recording GPS tracks](https://wiki.openstreetmap.org/wiki/Recording_GPS_tracks) | How to Record a GPS Track (#34) | The audience for this page seems to be mapping enthusiasts, which is a throwback to an earlier era when GPS technology was less commonplace. There is no mention of apps that do similar things, like Strava or MapMyRun, and whether such apps could be used to upload routes to OSM. The term "GPS track" may have been accurate decades ago, but plain language allows for terms like "route" and this would make the text easier to understand. | Usable, Helpful, Readable| Luigi Benetton |
| [Upload GPS tracks](https://wiki.openstreetmap.org/wiki/Upload_GPS_tracks) | How to Upload a GPS Track (#35) | Certain instructions (e.g., the "Browse" button) are outdated and no longer match the interface. The page contains troubleshooting information that could be better included in a “site-wide” troubleshooting page. The one image is so tiny it's incomprehensible and thus useless. The list of applications that support direct upload of GPS traces seems out of date and probably not worth updating, since the apps that meet this requirement will probably expand continuously. | Usable, Helpful, Visual | Luigi Benetton |
| [API v0.6](https://wiki.openstreetmap.org/wiki/API_v0.6) | capabilities (#36), map (#37), notes (#38), node/#id (#39) | About 70 endpoints on one very long page, so basic read operations are hard to find; endpoint sections don't follow a consistent structure (e.g., map has no Response subsection); limits explained in a different section; history notes and informal remarks mixed into reference content; the notes endpoint shows XML and JSON examples without explaining the fields (for example, what `status` means) | Searchable, Usable, Comprehensive | Kadria, Ashna, Macwilliam, Anna |

## Key findings across all pages

> **Draft:** based on the pages audited so far. Confirm, edit, or add findings when every page above is complete.

| # | Finding | Criteria affected | How our new documentation fixes it |
|---|---|---|---|
| 1 | **Topic types are mixed.** Steps, explanations, and technical reference are combined on the same page or in the same section. | Usable, Readable | Every topic follows one template only: Concept, Task, or Reference. |
| 2 | **Missing or incomplete steps.** Many how-to sections describe a feature but do not say exactly what to click or what happens next. | Comprehensive, Helpful | Tasks have Prerequisites, numbered Steps (one action each), Result, and Example. |
| 3 | **Few or unclear visuals.** Some pages have no images; others rely on numbered callouts on a single screenshot. | Visual, Accessible | Where helpful, topics include screenshots or diagrams with descriptive alt text. Interface controls are clearly identified in the instructions. |
| 4 | **Unexplained jargon.** Terms such as Nominatim, Mapnik, slippy map, and bbox appear without explanation. | Translatable, Readable | Plain language for beginners; OSM terms are defined on first use and collected in a glossary. |
| 5 | **Hard to find.** Content is buried in long pages that serve several audiences. | Searchable | One topic per Wiki page, with audience-based navigation in the sidebar on the Wiki home page. |
| 6 | | | |
