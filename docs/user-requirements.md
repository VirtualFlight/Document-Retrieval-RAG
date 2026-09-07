# User Requirements Document (URD)
## SR&T Intelligent Deal & Risk Assistant

**Version:** 1.0  
**Date:** September 2026  

---

## User Stories

### Document Upload & Management

- As a user, I should be able to upload PDF and Word documents (deal memos, risk reports) through the web interface.
- As a user, I should be able to see a list of all documents I have uploaded.
- As a user, I should be able to associate each document with a specific deal.
- As a user, I should be able to view the status of a document (e.g., "Uploaded", "Processing", "Ready").

### Deal Data Management

- As a user, I should be able to view a list of all deals in the system.
- As a user, I should be able to see key details for each deal (name, industry, deal value, risk level).
- As a user, I should be able to filter deals by industry.
- As a user, I should be able to filter deals by risk level (Low, Medium, High).
- As a user, I should be able to sort deals by deal value.

### Conversational Q&A (RAG)

- As a user, I should be able to type a natural-language question about my deals or documents into a chat interface.
- As a user, I should be able to see citations with each answer (document name, section, page number).
- As a user, I should be able to click on a citation to understand which document the answer came from.
- As a user, I should be able to ask follow-up questions in the same conversation.
- As a user, I should be able to start a new conversation at any time.

### Search & Discovery

- As a user, I should be able to search for relevant information across all my uploaded documents.
- As a user, I should be able to search within a specific deal's documents.
- As a user, I should be able to find documents that mention specific keywords (e.g., "regulatory risk", "covenants").

### Analytics & Dashboards

- As a user, I should be able to view a dashboard showing total deal value broken down by industry.
- As a user, I should be able to view a dashboard showing the number of deals by risk level.
- As a user, I should be able to see a KPI card showing the total portfolio deal value.
- As a user, I should be able to export or screenshot dashboard visuals for use in presentations.

### System Accessibility

- As a user, I should be able to access the application through a web browser (no installation required).
- As a user, I should be able to access the live demo without needing to create an account (for MVP).

---

## Priority Matrix

| Priority | User Stories |
|----------|--------------|
| **Must Have (MVP)** | Upload documents, view deals list, ask questions via chat, see cited answers, view Power BI dashboard screenshots, access live demo URL |
| **Should Have** | Filter/sort deals, search within specific deals, follow-up questions in conversation, click citations for more context |
| **Nice to Have** | Export dashboard visuals, conversation history, document status indicators |
| **Out of Scope (for MVP)** | User authentication, multi-tenancy, advanced agent workflows, mobile responsiveness |

---