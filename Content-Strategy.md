# Content Strategy – OpenStreetMap Beginner Documentation

**Team:** Copy Editors' Crusade
**Status:** DRAFT – for team review, then instructor approval
**Last updated:** 31 October 2026

> Sections marked **TO DO** need team input. Do not submit to the instructor until every TO DO is resolved.

### Open items at a glance

| # | Open item | Section |
|---|---|---|
| 1 | Problems identified – fill in after the audit is complete | 3 |
| 2 | Who assembles and publishes the Swagger project | 5, 6 |
| 3 | Peer reviewer for each writer | 6 |
| 4 | Owners for the Wiki sidebar and consistency check, and for the bonus video | 6 |
| 5 | Agree on the internal deadlines | 8 |
| 6 | Questions for the instructor | 10 |

---

## 1. Project overview

We are overhauling part of the [OpenStreetMap (OSM) Wiki](https://wiki.openstreetmap.org/wiki/Main_Page) beginner documentation. We will rewrite selected pages as separate concept, task, and reference topics in our GitHub Wiki, and improve the documentation for selected OSM API endpoints in Swagger.

## 2. Target audience

These are the three audiences defined in our approved proposal.

| Audience | Technical level | What they do | What they need |
|---|---|---|---|
| **General users** | Basic: comfortable using a web browser | View and use the map on openstreetmap.org | Short, clear steps; plain language; screenshots |
| **Beginner mappers** | Basic: no mapping, GIS, or programming experience | Create an account and make their first edits | Short, clear steps; explanations of OSM terms; screenshots |
| **Software developers** (API topics only) | Experienced | Use OSM data in their own applications | Straightforward API documentation with examples |

Our Wiki topics serve general users and beginner mappers. Our Swagger documentation serves developers.

## 3. Problems identified in the current documentation

Summary of the [audit](Audit.md).

> **TO DO – filled in after the audit.** This section depends on the audit, so it is completed once every writer has audited their source pages. Use only the audit findings recorded in the issue comments.

| # | Problem | Example page | Impact on beginners |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

## 4. Content principles and style rules

These rules follow the instructor's templates and his [write-the-docs writing rules](https://github.com/JordanStanchev/Getting-Started-as-User-Assistance-Developer/wiki/write-the-docs).

1. **One topic = one Wiki page.** The Wiki page title must match the issue title exactly.
2. **Keep information types separate.** Use the instructor's templates:
   - **Concept** answers "What is this?" (Summary, Detailed Overview, Example)
   - **Task** answers "How do I do this?" (Summary, Prerequisites, Steps, Result, Example)
   - **Reference** answers "What are the facts?" (Summary, then a reference heading, usually a table)
3. If a task needs a lot of explanation, create a separate concept topic and link to it. Instead of repeating concept text in a task, add a one-sentence summary and a link to the concept, so each page stays one information type.
4. **Steps:** numbered, one action per step, starting with a verb (*Click*, *Type*, *Select*).
5. **Language:** plain English, short sentences, no unexplained jargon. Define OSM terms the first time they are used.
6. **Formatting:** UI elements in **bold**, for example **Share**, **Layers**.
7. **Images:** at least one screenshot or diagram per topic that explains a feature, a step, or a concept. Highlight the important area. Give every image a descriptive alt text and a numbered caption in italics under it (*Figure 1. …*). Avoid decorative images that don't help the reader.
8. **Links:** each task links to its related concept, and each concept links to related tasks.
9. **Page titles:** task titles start with "How to" followed by an action (*How to Add a Missing Place*). Concepts and references use a clear, descriptive noun phrase (*OSM Data Elements: Nodes, Ways and Relations*, *OSM Glossary for Beginners*). Titles stay the same in the issue, the Wiki page and the sidebar.
10. **Results:** the Result section describes what the user sees or has when the task is complete.
11. **Examples:** use real, specific values, not placeholders.
12. **Testing:** test every task on openstreetmap.org before documenting it. Go through the steps, take screenshots, and close without saving, so nothing changes on the real map. In the iD editor, undo any test edits and never upload them.

## 5. New information structure

Our topics are grouped into five bundles. Each bundle becomes one group in the Wiki sidebar, and the Wiki **Home** page is the entry point. Each bundle contains 1 concept, 1 reference, and 3 tasks: 25 topics in total (5 concepts, 15 tasks, 5 references).

### Viewing the map (Bundle A)
| Topic | Type | Source page | Issue |
|---|---|---|---|
| What is OpenStreetMap? | Concept | About OpenStreetMap | #11 |
| Available Map Layers | Reference | Browsing › Layers | #12 |
| How to Find a Place on the Map | Task | Browsing › Finding Places | #13 |
| How to Switch Map Layers | Task | Browsing › Layers | #14 |
| How to Share a Map Link | Task | Browsing › Sharing a link to the maps | #15 |

### Map notes (Bundle B)
| Topic | Type | Source page | Issue |
|---|---|---|---|
| What Are Map Notes? | Concept | Notes | #16 |
| Map Note Markers and Statuses | Reference | Notes | #17 |
| How to View Notes on the Map | Task | Notes › Viewing notes | #18 |
| How to Resolve a Note | Task | Notes › Resolving notes | #19 |
| How to Add a Note to the Map | Task | Notes › Adding notes | #20 |

### Getting started with editing (Bundle C)
| Topic | Type | Source page | Issue |
|---|---|---|---|
| OSM Data Elements: Nodes, Ways and Relations | Concept | Beginners Guide 1.3 › The elements | #21 |
| OSM Glossary for Beginners | Reference | Glossary | #22 |
| How to Create an OSM Account | Task | OpenStreetMap account › Creating an Account | #23 |
| How to Add a Missing Place | Task | Beginners Guide 1.3 › Learn the basics of an editor | #24 |
| How to Edit an Existing Place | Task | iD › How to use it | #25 |

### Tags and features (Bundle D)
| Topic | Type | Source page | Issue |
|---|---|---|---|
| Tags and Map Features | Concept | Map features | #26 |
| Common Map Feature Tags | Reference | Map features › Primary features | #27 |
| How to Add Tags to a Feature | Task | Map features | #28 |
| How to Draw a Building | Task | Buildings › How to map | #29 |
| How to Add an Address | Task | Addresses › How to map | #30 |

### Saving and field mapping (Bundle E)
| Topic | Type | Source page | Issue |
|---|---|---|---|
| Armchair vs Outdoor Mapping | Concept | Pick your mapping technique | #31 |
| iD Keyboard Shortcuts | Reference | iD/Shortcuts | #32 |
| How to Upload Your Changes | Task | Beginners Guide 1.4.2 › Uploading your changes to OSM | #33 |
| How to Record a GPS Track | Task | Recording GPS tracks › How-to guide | #34 |
| How to Upload a GPS Track | Task | Upload GPS tracks › How to upload a GPS trace | #35 |

The full source links are in the topic bundles file and in each issue.

### OSM API (Swagger)

**Audience:** software developers. **Source:** [API v0.6](https://wiki.openstreetmap.org/wiki/API_v0.6). The endpoints are documented in a new Swagger (OpenAPI) project, not in the Wiki. They are tracked on the Project board with the topic type **API Endpoint**.

| Endpoint | What it does | Source section | Issue |
|---|---|---|---|
| GET /api/0.6/capabilities | Returns the API's limits and current status | 2.1.2 | #36 |
| GET /api/0.6/map | Returns the map data inside a bounding box | 2.1.3 | #37 |
| GET /api/0.6/notes | Returns the map notes inside a bounding box | 2.7.1 | #38 |
| GET /api/0.6/node/{id} | Returns the data for a single map point | 2.4.2 | #39 |

Each endpoint includes a plain-language summary, its parameters, a sample request and response, and its error codes. All four are read-only, so they can be tested safely.

**TO DO:** Agree who assembles the four endpoints into one Swagger project and publishes it.

## 6. Roles and responsibilities

Each writer owns one bundle (1 concept, 1 reference, 3 tasks). Four writers also own one API endpoint.

| Team member | Topics (writer) | API endpoint | Reviews topics of | Extra responsibility |
|---|---|---|---|---|
| Anna Ovsiannikova | Bundle D (#26–#30) | GET /api/0.6/node/{id} (#39) | **TO DO** | |
| Ashna Ayaz | Bundle A (#11–#15) | GET /api/0.6/map (#37) | **TO DO** | GitHub repository and Project board; Content Strategy draft |
| Kadria Hussein | Bundle C (#21–#25) | GET /api/0.6/capabilities (#36) | **TO DO** | Content Strategy review |
| Luigi Benetton | Bundle E (#31–#35) | – | **TO DO** | Presentation slides |
| Macwilliam Kwabena Appianing | Bundle B (#16–#20) | GET /api/0.6/notes (#38) | **TO DO** | |

Every team member records their own AI use in [AI-logs.md](AI-logs.md).

**TO DO:** Assign:
- the reviewer for each writer
- Swagger assembly and publishing
- the Wiki sidebar and consistency check
- the bonus video (optional)

## 7. Workflow

1. Each topic is tracked as an **issue** on the Project board: **Todo → In progress → In review → Done**.
2. The writer audits the original page and records it on the topic's issue: the issue description gives the source, scope and audience, then one comment for each key finding (tagged with the instructor's quality criteria, such as *Helpful*, *Usable* or *Readable*, with one or two "before" screenshots), and a final comment, "What I will fix".
3. The writer tests the task on openstreetmap.org, then creates the topic in the **Wiki** using the instructor's template. Wiki pages need no branches or pull requests.
4. The writer comments "Wiki page ready for review: [link]" on the issue, moves it to **In review**, and @mentions the reviewer.
5. The reviewer comments on the issue using the review checklist in [Peer-Review-Summary.md](Peer-Review-Summary.md).
6. The writer fixes the page and moves the issue to **Done**.
7. Repo files (strategy, Swagger, AI log) are changed on a personal branch through **pull requests**, reviewed and merged by a teammate. Audits do not need branches or pull requests.

## 8. Timeline

**TO DO:** Team to confirm these dates.

| Dates (2026) | Phase |
|---|---|
| Oct 28–30 | Assign topics; audit the source pages |
| Oct 31 | Complete the Content Strategy (problems section) after the audit |
| Oct 31 – Nov 1 | Write topics; draft API endpoints |
| Nov 2 | Peer review |
| Nov 3 | Final polish, Wiki sidebar, Swagger project published |
| Nov 4 | Slides, rehearsal |
| **Nov 5** | **Final presentation** |

## 9. Success criteria

- All topics follow the instructor's templates and writing rules.
- Each team member has written 1 concept, 3 tasks, and 1 reference.
- Every original page has an audit comment with a "before" screenshot on its issue.
- Every topic has a visible peer review on its issue.
- Every topic includes at least one new or updated image.
- The Wiki sidebar reflects the structure in section 5.
- The four selected API endpoints are documented in Swagger.
- AI usage is logged and verified.

## 10. Open questions for the instructor

**Answered:** The number of topics is flexible. The team has agreed on 25 topics in five bundles.

**TO DO:** Ask the instructor:

1. Does peer review in **issue comments** count as evidence, given that Wiki edits don't use pull requests?
2. For "a new Swagger project," should we submit an `openapi.yaml` file, a SwaggerHub link, or both?
