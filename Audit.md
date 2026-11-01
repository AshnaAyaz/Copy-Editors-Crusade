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
| [Browsing](https://wiki.openstreetmap.org/wiki/Browsing) | How to Add a Marker to a Shared Map (#18) | | | Macwilliam Appianing |
| [Notes](https://wiki.openstreetmap.org/wiki/Notes) | What Are Map Notes? (#16), How to Report a Map Problem with a Note (#20) | | | Macwilliam Appianing |
| [OSMF Attribution Guidelines](https://osmfoundation.org/wiki/Licence/Attribution_Guidelines) | OSM Attribution Requirements (#17) | | | Macwilliam Appianing |
| [Using OpenStreetMap](https://wiki.openstreetmap.org/wiki/Using_OpenStreetMap) | How to Export a Map Image (#19) | | | Macwilliam Appianing |
| [Beginners Guide 1.3](https://wiki.openstreetmap.org/wiki/Beginners_Guide_1.3) | OSM Data Elements: Nodes, Ways and Relations (#21), How to Add a Missing Place (#24) | | | Kadria Hussein |
| [Glossary](https://wiki.openstreetmap.org/wiki/Glossary) | OSM Glossary for Beginners (#22) | | | Kadria Hussein |
| [OpenStreetMap account](https://wiki.openstreetmap.org/wiki/OpenStreetMap_account) | How to Create an OSM Account (#23) | | | Kadria Hussein |
| [iD](https://wiki.openstreetmap.org/wiki/ID) | How to Edit an Existing Place (#25) | | | Kadria Hussein |
| [Map features](https://wiki.openstreetmap.org/wiki/Map_features) | Tags and Map Features (#26), Common Map Feature Tags (#27), How to Add Tags to a Feature (#28) | | | Anna Ovsiannikova |
| [Buildings](https://wiki.openstreetmap.org/wiki/Buildings) | How to Draw a Building (#29) | | | Anna Ovsiannikova |
| [Addresses](https://wiki.openstreetmap.org/wiki/Addresses) | How to Add an Address (#30) | | | Anna Ovsiannikova |
| [Pick your mapping technique](https://wiki.openstreetmap.org/wiki/Pick_your_mapping_technique) | Armchair vs Outdoor Mapping (#31) | | | Luigi Benetton |
| [iD/Shortcuts](https://wiki.openstreetmap.org/wiki/ID/Shortcuts) | iD Keyboard Shortcuts (#32) | | | Luigi Benetton |
| [Beginners Guide 1.4.2](https://wiki.openstreetmap.org/wiki/Beginners_Guide_1.4.2) | How to Upload Your Changes (#33) | | | Luigi Benetton |
| [Recording GPS tracks](https://wiki.openstreetmap.org/wiki/Recording_GPS_tracks) | How to Record a GPS Track (#34) | | | Luigi Benetton |
| [Upload GPS tracks](https://wiki.openstreetmap.org/wiki/Upload_GPS_tracks) | How to Upload a GPS Track (#35) | | | Luigi Benetton |
| [API v0.6](https://wiki.openstreetmap.org/wiki/API_v0.6) | capabilities (#36), map (#37), notes (#38), node/#id (#39) | About 70 endpoints on one very long page, so basic read operations are hard to find; endpoint sections don't follow a consistent structure (e.g., map has no Response subsection); limits explained in a different section; history notes and informal remarks mixed into reference content | Searchable, Usable, Comprehensive | Kadria, Ashna, Macwilliam, Anna |

## Key findings across all pages

> **Draft:** based on the pages audited so far. Confirm, edit, or add findings when every page above is complete.

| # | Finding | Criteria affected | How our new documentation fixes it |
|---|---|---|---|
| 1 | **Topic types are mixed.** Steps, explanations, and technical reference are combined on the same page or in the same section. | Usable, Readable | Every topic follows one template only: Concept, Task, or Reference. |
| 2 | **Missing or incomplete steps.** Many how-to sections describe a feature but do not say exactly what to click or what happens next. | Comprehensive, Helpful | Tasks have Prerequisites, numbered Steps (one action each), Result, and Example. |
| 3 | **Few or unclear visuals.** Some pages have no images; others rely on numbered callouts on a single screenshot. | Visual, Accessible | Each topic has its own screenshots or diagrams, with alt text, and buttons are named in the text. |
| 4 | **Unexplained jargon.** Terms such as Nominatim, Mapnik, slippy map, and bbox appear without explanation. | Translatable, Readable | Plain language for beginners; OSM terms are defined on first use and collected in a glossary. |
| 5 | **Hard to find.** Content is buried in long pages that serve several audiences. | Searchable | One topic per Wiki page, grouped by audience in a sidebar menu. |
| 6 | | | |
