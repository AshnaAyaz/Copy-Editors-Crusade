# Content Strategy – OpenStreetMap Beginner Documentation

**Team:** Copy Editors' Crusade
**Status:** DRAFT – for team review, then instructor approval
**Last updated:** <!-- date -->

> Sections marked **TO DO** need team input. Do not submit to the instructor until every TO DO is resolved.

---

## 1. Project overview

We are overhauling part of the [OpenStreetMap (OSM) Wiki](https://wiki.openstreetmap.org/wiki/Main_Page) beginner documentation. We will rewrite selected pages as separate concept, task, and reference topics in our GitHub Wiki, and improve the documentation for selected OSM API endpoints in Swagger.

## 2. Target audience

**Primary audience:** Beginners who are new to OpenStreetMap.

| Attribute | Description |
|---|---|
| Who they are | People who want to view, use, or start contributing to OSM |
| Technical level | Comfortable using a web browser; no mapping, GIS, or programming experience |
| Goals | Find places on the map, share maps, understand OSM data, start mapping |
| Needs | Short, clear steps; plain language; screenshots; explanations of OSM terms |

**Secondary audience (API topics only):** Developers who are new to the OSM API.

**TO DO:** Confirm the audience as a team.

## 3. Problems identified in the current documentation

Summary of the [audit](Audit.md).

**TO DO:** Fill in after the audit is complete. Use only findings recorded in Audit.md.

| # | Problem | Example page | Impact on beginners |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

## 4. Content principles and style rules

1. **One topic = one Wiki page.**
2. **Keep information types separate.** Use the instructor's templates:
   - **Concept** answers "What is this?" (Summary, Detailed Overview, Example)
   - **Task** answers "How do I do this?" (Summary, Prerequisites, Steps, Result, Example)
   - **Reference** answers "What are the facts?" (Summary, then a reference heading, usually a table)
3. If a task needs a lot of explanation, create a separate concept topic and link to it. A short piece of concept text may be repeated in a task so readers don't have to switch pages.
4. **Steps:** numbered, one action per step, starting with a verb (*Click*, *Type*, *Select*).
5. **Language:** plain English, short sentences, no unexplained jargon. Define OSM terms the first time they are used.
6. **Formatting:** UI elements in **bold**, for example **Share**, **Layers**.
7. **Images:** at least one screenshot or diagram per topic. Highlight the important area. Add a short description for every image.
8. **Links:** each task links to its related concept, and each concept links to related tasks.
9. **Page titles:** tasks start with a verb in -ing form (*Finding a place*); concepts and references use a noun phrase (*Armchair mapping*).

## 5. New information structure

Proposed Wiki navigation (sidebar). **TO DO:** Team to confirm the groups and add the extra topics.

### Getting started
| Topic | Type | Source page |
|---|---|---|
| History of OpenStreetMap | Reference | History of OpenStreetMap |
| What is OSM data? | Reference | Beginners Guide 1.3 |
| Joining the OSM community | Task | Join the community |
| Installing a desktop editor | Task | Beginners Guide 1.3 |

### Browsing the map
| Topic | Type | Source page |
|---|---|---|
| Finding a place | Task | Browsing |
| Understanding layers | Concept | Browsing |
| Switching between layers | Task | Browsing |
| Adding a marker | Task | Browsing |
| Sharing a map | Task | Browsing |
| Creating shortlinks | Task | Browsing |

### Choosing how to map
| Topic | Type | Source page |
|---|---|---|
| Armchair mapping | Concept | Pick your mapping technique |
| Outdoor mapping | Concept | Pick your mapping technique |

### Understanding OSM data
| Topic | Type | Source page |
|---|---|---|
| Elements of OSM data | Concept | Beginners Guide 1.3 |
| Tags in OSM data | Concept | Beginners Guide 1.3 |
| Primary features versus additional properties | Concept | Map features |
| Tagging a feature | Task | Map features |

### OSM API
| Topic | Type | Location |
|---|---|---|
| 2–4 API endpoints (to be chosen) | Reference | Swagger |

### Topic count check

| | Current | Required |
|---|---|---|
| Total topics | 16 | About 30 (brief) or 15 (workflow table). **TO DO:** confirm with the instructor |
| Concepts | 6 | At least 6 (1 per person) |
| Tasks | 8 | At least 12 (2 per person) |
| References | 2 | At least 6 (1 per person) |

**TO DO:** Add at least **4 tasks** and **4 references** to meet the per-person minimum. Candidate sources include the same OSM Wiki pages above.

## 6. Roles and responsibilities

**TO DO:** Fill in at the team meeting. Each person writes at least 2 tasks, 1 concept, and 1 reference.

| Team member | Topics (writer) | Reviews topics of | Extra responsibility |
|---|---|---|---|
| Anna Ovsiannikova | | | |
| Ashna Ayaz | | | |
| Belem | | | |
| Kadria | | | |
| Luigi Benetton | | | |
| Macwilliam Kwabena Appianing | | | |

Extra responsibilities to assign: Content Strategy, Swagger API, Wiki sidebar and consistency check, presentation, video, AI usage log.

## 7. Workflow

1. Each topic is tracked as an **issue** on the Project board: **Todo → In progress → In review → Done**.
2. The writer audits the original page and comments the findings and a "before" screenshot on the issue.
3. The writer creates the topic in the **Wiki** using the instructor's template.
4. The writer links the Wiki page in the issue and moves it to **In review**.
5. The reviewer comments on the issue using the review checklist in [Peer-Review-Summary.md](Peer-Review-Summary.md).
6. The writer fixes the page and moves the issue to **Done**.
7. Repo files (strategy, audit, Swagger) are changed through **pull requests** approved by a teammate.

## 8. Timeline

**TO DO:** Adjust to the instructor's checkpoint dates.

| Dates (2026) | Phase |
|---|---|
| Oct 24–25 | Assign topics, audit, draft content strategy |
| Oct 26–27 | Content strategy approval |
| Oct 27 – Nov 1 | Write topics |
| Oct 30 – Nov 2 | Peer review, Swagger API documentation |
| Nov 3–4 | Final polish, Wiki sidebar, slides, video, rehearsal |
| **Nov 5** | **Final presentation** |

## 9. Success criteria

- All topics follow the instructor's templates.
- Each team member has written at least 1 concept, 2 tasks, and 1 reference.
- Every topic has a visible peer review on its issue.
- Every topic includes at least one new or updated image.
- The Wiki sidebar reflects the structure in section 5.
- 2–4 API endpoints are documented in Swagger.
- AI usage is logged and verified.

## 10. Open questions for the instructor

1. Is the target about **30 topics** or **15 topics** per group?
2. Does peer review in **issue comments** count as evidence, given that Wiki edits don't use pull requests?
3. For "a new Swagger project," should we submit an `openapi.yaml` file, a SwaggerHub link, or both?
