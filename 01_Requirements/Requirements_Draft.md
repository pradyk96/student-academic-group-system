Requirements List — Draft v0.1
Prepared by: Pratyaksh Kumar | Coordinator: Tomas Jonušas
Source: "Participant's yearly workflow" (v0.1) + internship assignment

1. Record types
| Record | Purpose | Key fields |
|---|---|---|
| Interest | Chosen field and starting curiosity | Field, description, languages, rhythm |
| Field map | Shared overview of a research field | Origins, authors, sources, concepts, methods, findings, disagreements, open questions, search profile |
| Question | Question shared with the group | Question, context, related sources, author |
| Source | Bibliographic entry | Bibliographic data, DOI/link, access status, annotation |
| Research idea | Planned study | Question, rationale, material, method, scope |
| Meeting note | Record of a review meeting | Date, participants, agreed next step |

Every record also stores: origin (person/AI), review status, created and updated dates, links to related records.

2. Review status
AI draft → proposed for review → reviewed and included.
Disputed or outdated records return to review. AI never approves its own content.

3. Access levels
| Level | Who sees it | Examples |
|---|---|---|
| Private | Author only | Working notes, question drafts |
| Group | All members | Field maps, shared questions |
| Chosen audience | Selected people | Research ideas, text drafts |
| Public | Anyone | Nothing by default |

4. Library and copyright
Bibliographic records kept separate from full-text files.
Full texts of others' works only in private part. Public part holds references, links, own annotations.

5. AI agent tasks
1. Draft an initial field map with verifiable references and marked gaps
2. Build a search profile per field
3. Run a monthly scan, add candidates to a review area, write a digest
4. Suggest links between members' records, with a reason
5. State whether it analysed full text, abstract, or bibliographic data only

6. Design principles
Content independent of tool · configuration over code · low maintenance ·
iterate then fix · every decision documented with "how to change it" · bilingual (LT/EN)

Open questions
- [ ] How often should members update the system? (weekly / monthly / quarterly)
- [ ] Database access: Scopus / Web of Science status
- [ ] Final tool decision — deferred until the model is reviewed
- [ ] Where do members' personal areas sit inside the whole?
