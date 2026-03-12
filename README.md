# ⚡ AI-Powered Customer Support & Service Automation

> A Salesforce-inspired web application demonstrating AI-enabled inspection management and customer support automation using Agentforce, Prompt Builder, and Lightning App Builder concepts.

![Salesforce](https://img.shields.io/badge/Salesforce-00A1E0?style=for-the-badge&logo=salesforce&logoColor=white)
![Einstein AI](https://img.shields.io/badge/Einstein_AI-Agentforce-7526e3?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## 📌 Project Overview

This project demonstrates a fully functional **AI-Powered Customer Support & Service Automation** system built on Salesforce principles. It showcases the implementation of:

- Custom Salesforce Objects (User Case, Customer, Order, Merchandise, Knowledge)
- AI Summary generation via **Salesforce Prompt Builder** (Field Generation Template)
- **Agentforce / Einstein AI** integration for automated inspection summaries
- Lightning App Builder-style UI with record detail pages
- Role-based security model, validation rules, and field-level security concepts

---

## 🚀 Features

| Feature | Description |
|---|---|
| 🗂️ **User Cases** | Create & manage inspection/support cases with status, priority, inspector |
| 👤 **Customers** | Full customer records linked to cases and orders |
| 📦 **Orders** | Order management with customer and merchandise relationships |
| 🏷️ **Merchandise** | Product/service catalog management |
| 📚 **Knowledge Base** | Support articles with categories and publish status |
| ✨ **AI Summary (Prompt Builder)** | One-click AI-generated inspection summaries using MetaDataInspection template |
| 🤖 **Live Prompt Tester** | Test the Prompt Builder template with custom inputs |
| 📊 **Dashboard** | Real-time stats: case counts, AI activity log, critical priority tracker |
| 🔒 **Security Setup** | Visual setup panel showing Einstein, FLS, profiles, validation rules status |

---

## 🗂️ Project Structure

```
ai-salesforce-project/
│
├── index.html              # Main application (single-file, no dependencies)
├── README.md               # Project documentation
├── docs/
│   └── project_documentation.docx   # Full project documentation (Word)
└── screenshots/
    └── (add your own screenshots here)
```

---

## 🛠️ Technology Stack

- **Platform:** Salesforce (Developer Org)
- **AI Features:** Salesforce Agentforce, Prompt Builder (Field Generation)
- **UI:** Lightning App Builder, Lightning Record Pages (Dynamic Detail Pages)
- **Frontend Demo:** HTML5, CSS3, Vanilla JavaScript
- **Fonts:** Sora, JetBrains Mono (Google Fonts)

---

## 📋 Salesforce Objects Created

| Object Label | API Name | Purpose |
|---|---|---|
| User Case | `User_Case__c` | Core inspection & support case management |
| Customer | `Customer__c` | Customer personal details and contact info |
| Order | `Order__c` | Customer order tracking |
| Merchandise | `Merchandise__c` | Product and service catalog |
| Knowledge | `Knowledge__c` | Support knowledge base articles |

---

## 🤖 Prompt Builder — MetaDataInspection Template

**Type:** Field Generation  
**Target Object:** User Case (`User_Case__c`)  
**Target Field:** AI Summary (`Ai_Summary__c`)  
**Status:** ✅ Active

```
Generate a clear and professional inspection summary using the provided inspection details.

Inspection Name: {!$Input:User_Case__c.Name}
Created Date:    {!$Input:User_Case__c.CreatedDate}
Status:          {!$Input:User_Case__c.Status__c}

Explain the inspection status, inspection date, and key observations.
Ensure the summary is easy to understand and suitable for business users.
```

---

## 🔐 Security Configuration

- ✅ **Profile-Based Access** — Custom profiles per team (Inspection, Support, Management)
- ✅ **Field-Level Security (FLS)** — AI Summary field restricted per role
- ✅ **Role Hierarchy** — Management visibility into subordinate records
- ✅ **Validation Rules** — Required fields enforced on all objects
- ✅ **Sharing Rules** — Cross-team record visibility where needed

---

## 📦 How to Run (Web Demo)

1. Clone or download this repository
2. Open `index.html` in any modern browser
3. No server, no dependencies, no installation needed

```bash
git clone https://github.com/EshaaNZed/ai-salesforce-project.git
cd ai-salesforce-project
# Open index.html in your browser
```

---

## 🗺️ Execution Roadmap

| Phase | Name | Description |
|---|---|---|
| Phase 1 | Requirement Analysis & Planning | Business requirements, AI use cases, project scope |
| Phase 2 | Backend Development & Configuration | Custom objects, fields, Prompt Builder setup |
| Phase 3 | UI/UX Development | Lightning App Builder, Dynamic Detail Pages |
| Phase 4 | Testing & Security | Functional testing, FLS, profiles, validation rules |
| Phase 5 | Deployment & Documentation | Final activation, docs, maintenance plan |

---

## 👥 Stakeholders

| Role | Responsibility |
|---|---|
| Project Sponsor | Business objectives & deliverable approval |
| Salesforce Admin | System configuration, Prompt Builder, security |
| Inspection Team | Primary end users — create & manage cases |
| Support Team | Review cases, provide customer assistance |
| Management | Reports & dashboards for visibility |
| IT Support | Maintenance & technical issue resolution |

---

## 📄 License

This project was created for educational and demonstration purposes as part of a Salesforce AI development learning project.

---

## 🙋‍♀️ Author

**EshaaNZed**  
[![GitHub](https://img.shields.io/badge/GitHub-EshaaNZed-181717?style=flat&logo=github)](https://github.com/EshaaNZed)
