
# 🚀 ProjectCaptain
### AI Project Knowledge Copilot for Enterprise Teams

ProjectCaptain is an **AI-powered project copilot** designed to help teams quickly understand project context, plan work, and retrieve critical information across enterprise systems.

Instead of manually searching across multiple platforms such as **Jira, Confluence, SharePoint, GitHub, and Teams**, ProjectCaptain provides a **single intelligent interface** that retrieves project knowledge and assists with project operations.

The goal is to reduce **onboarding friction, project management overhead, and context switching** across tools.

---

# 💡 Problem

Enterprise projects store critical knowledge across many platforms:

- Jira  
- Confluence  
- SharePoint  
- GitHub  
- MS Teams  
- ServiceNow  

New joiners and even experienced team members often spend **hours navigating different tools to understand project context**.

Common challenges include:

- Slow onboarding for new team members  
- Scattered documentation and project knowledge  
- Difficulty understanding ownership and dependencies  
- Inefficient sprint planning  
- Lack of a centralized project knowledge source  

ProjectCaptain addresses this by acting as a **central AI copilot for project knowledge and automation.**

---

# 🎯 What ProjectCaptain Does

ProjectCaptain assists teams across **three key areas**.

## 1️⃣ Instant Project Onboarding

New team members can quickly understand the project by asking natural language questions.

Example queries:

- What is the goal and scope of this project?
- Who owns integration testing?
- What are the key project dependencies?
- What systems are involved in the architecture?

This significantly reduces onboarding time from **weeks to minutes.**

---

## 2️⃣ Sprint Planning & Project Management Assistance

ProjectCaptain helps Scrum Masters and teams plan and manage work.

Example capabilities:

- Retrieve current sprint status from Jira
- Analyze backlog items
- Suggest sprint planning assignments
- Identify risks or blocked issues
- Generate RAID updates or weekly reports

Example query:

```

Help me plan the next sprint based on current backlog items

```

---

## 3️⃣ Document Intelligence

The assistant helps users understand project documentation.

Example queries:

- Explain the ERD for the Policy database
- Where is the source of truth for this user story?
- Summarize the latest architecture documentation

ProjectCaptain retrieves relevant documentation and generates a **context-aware explanation.**

---

# 🧠 How ProjectCaptain Works

ProjectCaptain uses a **retrieval-based AI architecture**.

The system connects to multiple enterprise systems and retrieves relevant information before generating responses.

```

User Question
│
▼
ProjectCaptain AI Copilot
│
▼
Context Retrieval Layer
│
▼
Enterprise Knowledge Sources
├── Jira API
├── Confluence API
├── SharePoint
├── GitHub
└── Project Documentation
│
▼
AI Reasoning + Response Generation

````

This approach ensures responses are **grounded in real project data instead of assumptions.**

---

# 🏗 Architecture

> 📌 Insert the system architecture diagram from the presentation here.

ProjectCaptain consists of three main components:

### 1️⃣ Data Sources

Enterprise systems providing project information.

Examples:

- Jira issues and backlog data
- Confluence documentation
- Architecture documents
- ERD and schema definitions
- Sprint summaries

---

### 2️⃣ Context Retrieval Layer

This layer retrieves relevant project context from connected systems.

Data is fetched through APIs and structured into retrievable knowledge objects.

Examples:

- Jira issue metadata
- Confluence page content
- Project documentation
- Schema definitions

---

### 3️⃣ AI Copilot

The AI layer analyzes retrieved information and generates responses for users.

Capabilities include:

- answering project questions
- summarizing documentation
- suggesting sprint plans
- identifying dependencies and risks

---

# 🔌 Integrations

ProjectCaptain connects to enterprise systems through APIs.

## Jira Integration

Jira issues are retrieved using the **Jira REST API** and structured into JSON objects.

Example:

```json
{
  "issue_key": "SCRUM-21",
  "summary": "Document RCA",
  "assignee": "Rituparna Dhar",
  "status": "To Do",
  "priority": "Medium"
}
````

This allows the AI assistant to analyze project work items and sprint activities.

---

## Confluence Integration

Confluence pages are retrieved through the **Confluence API** and converted into structured knowledge documents.

Example:

```
Page Title: Data Model Overview
Content: Explanation of entities, relationships, and schema design.
```

This enables the assistant to answer architecture and documentation-related questions.

---

# 📂 Repository Structure

```
projectcaptain/

data/
    jira_stories.json
    sprint_summaries.json
    erd_fields.json

docs/
    architecture_overview.md
    data_model_overview.md
    entity_relationships.md
    solution_approach.md

prompts/
    projectcaptain_prompt.md
    sprint_planning_prompt.md

README.md
```

---

# 💬 Example Questions

ProjectCaptain can answer questions such as:

### Project Context

```
What is the goal of this project?
```

```
Who owns the Policy database schema?
```

### Sprint Planning

```
Help me plan the next sprint
```

```
What issues are currently open in Jira?
```

### Documentation

```
Explain the ERD for the Policy database
```

```
Which sprint introduced the Claim Amount field?
```

---

# 📈 Impact

ProjectCaptain improves enterprise project workflows by:

* Accelerating onboarding for new team members
* Reducing time spent searching across tools
* Improving sprint planning and risk management
* Providing centralized project knowledge

Organizations benefit from:

* Faster productivity ramp-up
* Improved project transparency
* Better decision-making across teams

---

# ⚠️ Challenges

Some challenges when implementing AI assistants in enterprise environments include:

* Managing permission and security models
* Ensuring data freshness
* Resolving conflicting sources of truth
* Minimizing AI hallucinations

ProjectCaptain mitigates these challenges by relying on **retrieval-based responses grounded in trusted project sources.**

---

# 👥 Team

**Team 5 – Agent Xcelerate**

* Rituparna Dhar
* Jule Loescher
* Pradyumna Shivanandaiah
* Isha Verma

---

# 🏁 Hackathon Project

ProjectCaptain was developed as part of the **Reinvention with AI Hackathon** to demonstrate how AI copilots can transform **project onboarding, knowledge retrieval, and sprint planning** within enterprise environments.
