## AI usage – Ashna Ayaz

**Tool:** Claude (Anthropic)
**Period:** October 23 – November 2, 2026
**Topics:** What is OpenStreetMap? (#11), Available Map Layers (#12), How to Find a Place on the Map (#13), How to Switch Map Layers (#14), How to Share a Map Link (#15), GET /api/0.6/map (#37). Also coordinated the team's GitHub setup and the combined SwaggerHub documentation.

### Summary of use

| # | Area | What I asked for (prompt, summarized) | What the AI produced | How I verified it | What I changed or rejected |
|---|---|---|---|---|---|
| 1 | Learning GitHub | "How do we use Projects, issues, the Wiki, and pull requests? Why can't my teammates edit the board?" | Explanations of GitHub Projects, issues, Wiki, pull requests, roles, and rulesets | Tried each step in our repo; confirmed teammates could edit after I invited them with the Write role | Found that typing an email did not invite anyone; used GitHub usernames instead. Turned off the pull request rule after Jordan said PRs were not required |
| 2 | Planning the work | "Guide me through the steps to complete our project, from creating tasks to writing and delivering the documentation" (with the brief and proposal) | A workflow for each topic (issue, audit, Wiki page, review, done), a deliverable checklist, and a timeline | Compared it with the brief and Jordan's announcement | AI pointed out contradictions (30 vs 15 topics, missing team member); we confirmed with Jordan. Belem was not part of our team, so I removed Belem from all files |
| 3 | Project files | "Create README, Audit, Content Strategy, Peer Review Summary, and Deliverables files" | Markdown templates for the repo | Reviewed each file against the brief | Removed placeholder content we did not need; changed the audit to follow the eleven-point framework from our proposal, because the first version used a different set of criteria |
| 4 | Audit | "Audit my topics and the API page against our criteria" | Draft findings for each topic | Read each original OSM page myself and took "before" screenshots | AI marked uncertain points as "to verify"; I checked them. After I sent a screenshot of the original Capabilities section, AI dropped one claim ("fields are scattered") that was not accurate. We kept detailed audits in issue comments and only a summary in Audit.md |
| 5 | Wiki topics | "Guide me to create improved documentation for my Wiki topics, using Jordan's templates and my audit findings" | Draft concept, task, and reference pages | Tested every step on openstreetmap.org and compared with the templates | Several drafts did not match the live website and were corrected: there is no "Go" button (search uses a magnifying-glass button); the layer list had changed (ÖPNVKarte removed; Shortbread and MapTiler OMT added); overlay and panel names were updated; the Share panel options were added |
| 6 | Images | "Create an image for my What is OpenStreetMap page that shows how OpenStreetMap works," "Which screenshots do I need?" and "Can you take them?" | A diagram (How OpenStreetMap works: mappers → map data → maps and apps); a screenshot list for each page; some screenshots of openstreetmap.org | Checked that the diagram matched the page text and the original About OpenStreetMap page; checked each screenshot against the live website | Used the diagram as Figure 1 and added descriptive alt text. AI could not load most map layers, so I took the layer screenshots myself. I resized images and fixed the layout after peer review |
| 7 | API documentation | "Guide me to create improved API documentation for GET /map in OpenAPI for SwaggerHub" | An OpenAPI file for GET /map, with a description, benefit, how to use it, parameters, responses, and error codes | Compared with the original API v0.6 page and an independent library's documentation; the file passed an OpenAPI validator | Restructured descriptions to follow Jordan's guidance (what it does, benefit, how to use it). Rewrote my endpoint to match Macwilliam's style. Example responses are illustrative, not live data, as Jordan said live examples were out of scope |
| 8 | Combining team work | "Combine my and Macwilliam's API work" | One SwaggerHub file with both endpoints and a Wiki "API Reference" page | Checked that Macwilliam's wording was kept | Kept Macwilliam's endpoint as he wrote it; did not change his examples |
| 9 | Grammar and content check | "Check the grammar, clarity, and content of my Wiki pages and API documentation" | Suggested corrections for grammar, sentence length, consistent terms, and missing information | Read each suggestion against the original OSM pages and Jordan's templates before accepting it | Accepted fixes for grammar, broken links, and unclear wording; kept my own wording where the meaning was already clear; rejected changes that added content beyond the topic |
| 10 | Peer review fixes | "Resolve these review comments" | Corrected page content | Re-read each page after saving | Applied only the reviewer's requested changes and kept the rest of the page as written |



## AI usage, Macwilliam Appianing

**Tool:** Claude (Anthropic)
**Period:** October 23 to November 4, 2026
**Topics:** What Are Map Notes? (#16), Map Note Markers and Statuses (#17), How to View Notes on the Map (#18), How to Comment on a Note (#19), How to Add a Note to the Map (#20), GET /api/0.6/notes (#38). Also peer reviews of colleagues' pages.

### Summary of use

I used Claude as a tutor and a drafting partner, and I stayed in control of the work. **I chose the scope, set the style I wanted, tested everything on the live website, took the screenshots, and wrote the final text of my audits and wiki pages.

The table follows the order in which I worked: understanding GitHub and the team workflow, understanding the assignment, planning my own timeline, choosing topics, auditing, building the API documentation, writing the wiki pages, and combining my work.

| # | Area | What I asked for (prompt, summarized) | What the AI produced | How I verified it | What I changed or rejected |
|---|---|---|---|---|---|
| 1 | Planning my own timeline | **I asked the AI to help me plan my own order of work for my part, before the November 5 presentation: topics, audit, wiki pages, Swagger, peer review.** | A draft work plan with the order of steps | **I checked it against the deadline and the team plan** | **I changed the order to fit my own time, and I did the work in the order that suited me** |
| 2 | Audit and the quality framework | **I wrote the audit of the Notes page myself. Then I pasted my findings and prompted the AI to review them and confirm that they met Jordan's quality criteria (Helpful, Comprehensive, Usable, Visual, Readable, Searchable, Accessible), and that each finding had a clear fix.** I did this for each topic, for example when I asked it to polish my #19 audit after I changed the topic to "comment". | A review of my findings against the criteria, with suggested wording changes | **I read the original OSM page myself, took the "before" screenshots, and checked every finding and every suggestion against the page.** | I decided which suggestions to accept. The findings and the final audit text are mine. |
| 3 | Learning the API task | **"Treat the API part as a complete follow along course, so I do it step by step as I learn what needs to be done for the project."** I also asked it to refer to Jordan's slides. | A step by step guide for SwaggerHub and OpenAPI | **I followed each step in SwaggerHub and sent a screenshot of my screen at each point.** The guide was then corrected to what I really saw | **When the first audit and Swagger were too complex, I asked to reset: "For my first project I want my audit and Swagger to be very simple. Identify a simple thing and do a simple Swagger."** I also asked for the code in small batches, **"so I see exactly what changes and what it does"** |
| 4 | Building the Swagger documentation | **"The contact section is too messy. Keep it simple: if anyone needs information they can contact the API documentation team at my email, and they can visit our project page. Very clean, with the subheadings clearly bolded."** | An OpenAPI file for GET /api/0.6/notes with a summary, three parameters, a field table and XML and JSON examples | **I used Try it out and sent the real XML response file and screenshots of the XML and JSON views.** The AI could not open the OSM wiki itself, so **I supplied screenshots and PDFs of the wiki pages** | **I found that the XML example showed `&lt;` characters. The AI reproduced the problem and rebuilt the example from a schema.** I also showed a screenshot proving the AI wrong about when a tag appears, and it corrected itself |
| 5 | Combined audit file | **"Give me all my audits in one file", because the team will build one Audit report.** Later I pasted my compiled text and asked for it to be updated | One document with all my audits | **I compared each audit with what I had posted on the issues** | **I compiled the final text myself.** I asked for corrected headings, and for a plain text version I could paste |



## AI usage – Kadria Hussein

**Tool:** ChatGPT (OpenAI)  
**Period:** October–November 2026  
**Topics:** OSM Data Elements: Nodes, Ways and Relations (#21), OSM Glossary for Beginners (#22), How to Create an OSM Account (#23), How to Add a Missing Place (#24), How to Edit an Existing Place (#25), and GET /api/0.6/capabilities (#36). Also contributed to peer reviews and the team's project video.

### Summary of use

I used ChatGPT as a learning assistant, drafting partner, and second-level editorial reviewer throughout the project. My approach was iterative and varied depending on the task. In some cases, I drafted the content independently before asking AI to review and improve it; in others, I used AI to help develop an initial structure or draft, which I then revised and verified.

For peer reviews, I first examined my colleagues' documentation and identified potential issues myself, then consulted AI to check whether I had overlooked any meaningful problems.

AI suggestions were not accepted automatically. I evaluated them against the original documentation, actual interface behavior, assignment requirements, and my own editorial judgment.

The table summarizes my main prompt patterns and how I verified the results.

| # | Area | What I asked for (prompt, summarized) | What the AI produced | How I verified it | What I changed or rejected |
|---|---|---|---|---|---|
| 1 | Understanding the assignment and workflow | "Help me understand Jordan's documentation requirements and organize my work across the audits, Wiki pages, API documentation, and peer reviews." | Explanations of the required Concept, Task, and Reference structures, GitHub workflow, and project deliverables. | Compared the recommendations with the assignment, Jordan's templates, his forum answers, and the team's agreed workflow. | Adapted the suggested process to our team's decisions and avoided unnecessary work, such as treating pull requests as mandatory. |
| 2 | Auditing the original documentation | "Review my findings and the original OSM pages against our quality criteria. Identify any additional meaningful issues and suggest improvements." | Additional audit observations, explanations of usability problems, and possible corrections. | Examined the original pages, checked findings against the source content, and used screenshots as supporting evidence. | Refined or rejected findings that were too general, unsupported, or outside the scope. Recorded detailed findings in the corresponding GitHub Issues. |
| 3 | Writing the Wiki topics | "Review my draft or help me develop a structured explanation using Jordan's templates. Check clarity, completeness, terminology, and suitability for beginners." | Editorial suggestions, alternative wording, structured explanations, and, where needed, draft content. | Compared the suggestions with my original writing, OSM documentation, available screenshots, actual interface behavior, and Jordan's templates. | Retained my own wording where appropriate, incorporated useful improvements, corrected interface descriptions, and rejected unnecessary rewrites or unsupported information. |
| 4 | Screenshots and accessibility | "Help me decide where screenshots are needed, what to highlight, and how to write useful alt text and figure captions." | Suggestions for screenshot placement, annotations, captions, and accessibility descriptions. | Reviewed the images against the actual procedures and checked whether the annotations matched the surrounding instructions. | Adjusted visual references and wording when they did not match the screenshots or could confuse readers. |
| 5 | Learning and creating OpenAPI documentation | "Guide me step by step through SwaggerHub and help document GET /api/0.6/capabilities, including its request, response fields, and XML and JSON examples." | An OpenAPI YAML definition, field descriptions, response schemas, and guidance on using SwaggerHub. | Compared the documentation with the original API reference and live XML and JSON responses. Validated the specification in Swagger Studio with zero reported errors. | Corrected the response examples, clarified the timeout field, followed the team's Swagger style, and rejected an unsupported claim about an HTTP error response. |
| 6 | Peer review and final corrections | "I've reviewed this colleague's page and identified these issues. Is there anything else meaningful I may have missed, particularly regarding technical accuracy, Jordan's requirements, or usability?" | Additional observations, potential issues, and suggested wording for constructive review comments. | Checked each suggestion against the published Wiki page, screenshots, original references, and my own findings. | Accepted only meaningful corrections and avoided unnecessary editorial preferences. Rejected an incorrect AI observation about a figure caption after examining the complete screenshot. |
| 7 | Consolidated project documentation | "Help me organize a high-level audit summary and AI usage log consistent with the team's approach and Jordan's instructions." | Suggestions for linking audit Issues to improved Wiki pages and summarizing AI usage and human verification. | Checked Jordan's forum response and compared the suggestions with the team's shared files and decisions. | Kept the audit summary concise, with detailed evidence in individual Issues, and avoided a lengthy prompt-by-prompt AI log. |
| 8 | Project video | "Help me plan a short video showing the original documentation, audit findings, improved Wiki pages, and API documentation. Adapt the narration to my ActivePresenter slides." | A recording storyboard, narration scripts, SSML text-to-speech markup, and suggestions for visual annotations and transitions. | Created and reviewed the recordings in ActivePresenter, checked narration against the visible frames, and adjusted the sequence to demonstrate different documentation types. | Split the original recording into static frames for better control, revised narration that did not match the screen, and replaced a repeated Task example with a Concept example. |



## AI usage – Anna Ovsiannikova

Tool: Perplexity  
Period: November 3–5, 2026  
Topics: Tags and Map Features, How to Add an Address, GET /api/0.6/node/{id} (#39), and peer reviews.

### Summary of use

I used Perplexity to review articles and improve API documentation. It also helped me write feedback in English.

I shared texts, comments, and screenshots. The AI suggested changes. I asked for simple words and shorter sentences. I chose which points to include in my comments.

### Summary table

| # | Area | What I asked for | What the AI produced | How I checked it | What I changed or did not use |
|---|---|---|---|---|---|
| 1 | Topic templates | “Does this article follow the correct template?” | A review of the sections. An explanation of each template. | I asked the AI to check the project document again. | I asked for small changes, not a full rewrite. |
| 2 | My Wiki topics | “Explain this review comment. What should I change?” | Ideas for headings, sections, and related links. | I compared the ideas with the article and comment. | I focused on the requested changes. I left out extra content. |
| 3 | The API task | “Do I need to rewrite the existing block?” | An explanation of the task and existing work. | I shared screenshots of Swagger and the Wiki page. | The AI first suggested a new block. After seeing the screenshots, it suggested updating the existing one. |
| 4 | Node documentation | “Write the YAML. Follow my audit and the review comment.” | A draft with steps, fields, examples, and errors. | I asked the AI to compare it with my audit and the comment. It also checked OSM sources. | I asked for JSON details. The AI clarified `version`. It removed “fastest way” and corrected `visible` in JSON. |
| 5 | Shorter API text | “Remove repeats. Make the text shorter.” | Shorter descriptions. | I compared them with the required content. | I kept the steps, field table, and examples. I removed repeated warnings. |
| 6 | YAML checks | “Check the YAML with a validator or linter.” | A local check report and a YAML file. | I read the results for YAML, JSON, and XML. | I did not call this a full OpenAPI check. Live API responses were not confirmed. |
| 7 | Peer reviews | “Is this article clear? Does it follow the requirements?” | Reviews of team members’ articles. | I compared the suggestions with the shared texts. I confirmed that the note-marker table was readable. | I chose the main points. For the notes article, I kept only the comment about links. |
| 8 | English feedback | “Use friendly A2 English. Make it a suggestion.” | Short review comments. | I read each version. I asked for changes. | I chose simpler words and a softer tone. |
| 9 | AI usage log | “Use the same format as my team.” | A draft of this log. | I compared it with our conversation. | I kept completed checks separate from unconfirmed checks. I did not say the changes were published. |
