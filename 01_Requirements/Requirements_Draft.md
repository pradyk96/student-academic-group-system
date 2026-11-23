# Requirements List — Draft v0.1
**Date:** 23 November 2026  
**Prepared by:** Pratyaksh Kumar (Intern)  
**Coordinator:** Tomas Jonušas  
**Status:** Draft (Skeleton)  
**Source:** *"Participant's yearly workflow"* (v0.1) & Internhip Assignment Brief  

---

## 1. Record Types & Metadata Schema
The system must support the following core record types. Every record must automatically capture standard metadata:

| Record Type | Purpose | Key Fields & Metadata |
| :--- | :--- | :--- |
| **Interest** | Participant's chosen academic field and starting curiosity. | Field name, short description, languages, rhythm, origin (person/AI), review status, created/updated dates. |
| **Field Map** | Shared overview of a research field. | Sections (origins, authors, sources, concepts, methods, findings, disagreements, open questions), search profile, links to related records. |
| **Question** | A question shared with the group for discussion. | Question text, context, related sources, author, review status, links. |
| **Source** | Bibliographic entry in the group library. | Bibliographic data, DOI/link, access status, annotation, origin, review status. |
| **Research Idea** | Participant's planned study proposal. | Question, rationale, material, method, scope, author, review status, chosen audience. |
| **Meeting Note** | Short agreed record of a review meeting. | Date, participants, agreed next steps, links to related records. |

*All records must support standard metadata: origin (person or AI), review status, creation/update timestamps, and bidirectional links to related records.*

---

## 2. Review Workflow (Status Machine)
The lifecycle of a record is controlled to ensure quality. The workflow is as follows:

$$\text{AI Draft} \longrightarrow \text{Proposed for Review} \longrightarrow \text{Reviewed and Included}$$

*   **Rule 1:** Disputed or outdated records must return to the review stage.
*   **Rule 2:** The AI agent **never** approves its own content. Human coordinator validation is mandatory before publication.

---

## 3. Access Control Levels (ACLs)
Content visibility must be strictly controlled based on the record's sensitivity:

| Level | Visibility | Examples |
| :--- | :--- | :--- |
| **Private** | Author only. | Working notes, draft questions, personal logs. |
| **Group** | All verified group members. | Shared field maps, group questions, meeting notes. |
| **Chosen Audience** | Selected members designated by the author. | Draft research ideas, draft text chapters. |
| **Public** | Anyone (external viewers). | Nothing by default; must be explicitly decided and approved case-by-case. |

---

## 4. Library & Copyright Rules
*   **Separation of Concerns:** Bibliographic metadata must be stored separately from full-text files.
*   **Private Storage:** Full-text files of others' works (copyrighted material) must be stored **only** in the private area of the creator or designated admin for internal use.
*   **Public/Group View:** Public-facing and group-facing parts of the library must contain **only** references, links, and the group's own annotations. No raw copyrighted PDFs.

---

## 5. AI Agent Functional Requirements
The AI agent is a core component of the system. Its mandatory functions are:
1.  **Field Map Drafting:** Generate an initial field map draft from available sources, with verifiable references and explicitly marked knowledge gaps.
2.  **Search Profile Generation:** Build a structured search profile per field, including keywords, synonyms, and logical combinations.
3.  **Monthly Literature Scan:** Automatically run monthly scans, add new candidate sources to a review area, and write a structured digest per field.
4.  **Link Suggestion:** Proactively suggest links between members' shared records, providing a short, explainable reason for each proposed link.
5.  **Transparency Statement:** Explicitly state the level of analysis performed (full text, abstract, or bibliographic data only) for every generated output.

---

## 6. Core Design Principles
The system architecture must adhere strictly to the following principles:
1.  **Content Independence:** All content stored as plain text (Markdown with YAML frontmatter). The tool can be replaced; the content survives.
2.  **Configuration over Code:** Prioritise templates and settings. Any custom code must be minimal, documented, and isolated.
3.  **Low Maintenance:** After January, a member without IT training must be able to run, update, and maintain the system.
4.  **Iterate, Then Fix:** Test each part in real use before standardising it.
5.  **Documentation-Driven:** Every decision must be documented with a *"how to change it"* note.
6.  **Bilingual Support:** Structure and templates must support both Lithuanian and English natively.

---

## 7. Open Questions & Next Steps
*   [ ] Confirm the status of Scopus / Web of Science database access for the AI agent.
*   [ ] Define the exact file naming conventions for records (e.g., `YYYY-MM-DD_Author_Title.md`).
*   [ ] Define the sync frequency for members (weekly, monthly, or quarterly).
*   [ ] Schedule 2–3 interviews with group members to validate these requirements.
