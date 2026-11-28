# Requirements List — Draft v0.1
Date: 28 November 2026
-Prepared by: Pratyaksh Kumar
-Coordinator: Tomas Jonušas
-Source: Participant's yearly workflow (v0.1) + member interviews

## 1. Record Types
| Record | Purpose | Key Fields |
|---|---|---|
| Interest | Chosen field and curiosity | Field, description, languages, rhythm |
| Field map | Shared overview of a field | Origins, authors, sources, concepts, methods, findings, disagreements, open questions, search profile |
| Question | Question shared with group | Question, context, related sources, author |
| Source | Bibliographic entry | Bibliographic data, DOI/link, access status, annotation |
| Research idea | Planned study | Question, rationale, material, method, scope |
| Meeting note | Record of review meeting | Date, participants, agreed next step |
| AI-generated emotional content — Lithuanian student group

Every record stores: origin (person/AI), review status, creation/update dates, links to related records.

## 2. Review Status
AI Draft → Proposed for Review → Reviewed and Included.
AI never approves its own content. Disputed records return to review.

## 3. Access Levels
| Level | Who Sees It | Examples |
|---|---|---|
| Private | Author only | Working notes, question drafts |
| Group | All members | Field maps, shared questions |
| Chosen Audience | Selected people | Research ideas, text drafts |
| Public | Anyone | Nothing by default |

## 4. Library & Copyright
- Bibliographic records separate from full-text files.
- Full texts of others' works stored only in private part.
- Public part holds references, links, and group's own annotations.

## 5. AI Agent Tasks
1. Draft initial field map with verifiable references and marked gaps.
2. Build search profile (keywords, synonyms, combinations) per field.
3. Run monthly scan, add candidates to review area, write digest.
4. Suggest links between members' records with reason.
5. State whether it analysed full text, abstract, or bibliographic data only.

Database access: Scopus and Web of Science (subject to confirmation). Fallback: OpenAlex, Crossref, Semantic Scholar.

## 6. Design Principles
- Content independent of tool (Markdown + metadata).
- Configuration over custom code.
- Low maintenance (non-IT person can run after January).
- Iterate, then fix.
- Every decision documented with "how to change it".
- Bilingual (Lithuanian and English).

## 7. Open Questions
- [ ] How often should members update? (Weekly / Monthly / Quarterly)
- [ ] Status of Scopus / Web of Science access
- [ ] Tool decision: Obsidian vs GitHub (deferred)
