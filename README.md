# Hi there 👋, I'm Mike Hermans

**Senior Application Engineer @ Magnetek (Columbus McKinnon)**

I design and operate production multi-agent systems, document-intelligence pipelines, and Power Platform automation that turn complex industrial RFQs, specifications, drawings, and quote packages into structured, evidence-backed work for application engineers.

---

## What I Build

I work at the intersection of application engineering, industrial automation (crane & hoist control systems), Microsoft 365 / Power Platform, and applied multi-agent AI. The focus is practical impact: faster review cycles, stronger source discipline, fewer missed requirements, cleaner handoffs, and more repeatable quoting and process-improvement workflows.

Key areas:
- Governed multi-agent orchestration in Microsoft Copilot Studio (runtime fleet + meta/control plane)
- Document intelligence & RFQ/specification parsing with evidence preservation and structured outputs
- Power Platform workflow automation (Power Automate, Power BI, Dataverse, SharePoint, Teams)
- Reusable Skills, instruction libraries, handoff contracts, and agent-authoring toolkits
- Salesforce-connected quote workflow support and SharePoint case/folder automation
- Internal communities of practice (Better Way Builders) and governed idea-to-sustainment processes

---

## I.D.E.A. — Think Differently

![I.D.E.A. — Iterate. Demonstrate. Educate. Automate.](https://raw.githubusercontent.com/hermansmpjr/hermansmpjr/main/IDEA%20-%20Think%20Differently.png)

**I.D.E.A. = Iterate. Demonstrate. Educate. Automate.**

I.D.E.A. is the operating rhythm behind Better Way Builders, an internal improvement community where employees experiment with Copilot, Power Automate, Power BI, SharePoint, and related Microsoft 365 tools, then document and scale what works.

- **Iterate** — Identify a problem, opportunity, or hypothesis for improvement
- **Demonstrate** — Test the idea with a practical tool or workflow
- **Educate** — Document what worked, what failed, and what others can reuse
- **Automate** — Scale the solution when it is reliable, useful, and ready for broader adoption

The same cycle underpins the Event-Horizon framework and the agent-fleet-os patterns used across the MAG fleet.

---

## Current Focus Areas

### Two-Layer Multi-Agent Architecture

I maintain a governed multi-agent system with a clear separation of concerns:

**Production Runtime (MAG-Fleet)**  
The agents that perform customer/engineering work:
- **MAG-AutoPilot-AE-CS** — RFQ / application-engineering orchestrator (intake readiness, source diagnostics, engineering packet extraction, BOM/pricing support, compliance matrix, proposal export, Salesforce case lookup, etc.)
- **MAG-Electrical-Drawing-Interpreter** — Source-grounded extraction from electrical/crane drawings and motor data sheets (includes a dedicated Python OCR tool)
- **MAG-Compliance-Documenter** — Internal compliance & traceability reporting
- **MAG-Fleet-Documenter** & **MAG-Dev-Architect** — Documentation and architecture/routing parent for the runtime layer

**Meta / Control Plane (MAG-Fleet-Meta)**  
The agents that govern, generate, and improve the fleet:
- **MAG-Fleet-Governor** — Strategic oversight, routing decisions, hard rules, promotion authority
- **MAG-Agent-Factory** — Programmatic creation of new governed agents
- **MAG-Knowledge-Discovery** & **MAG-Knowledge-Mapper** — Source discovery, naming, overlap detection, connect-vs-tool classification
- **MAG-Agent-Intake-Guide** — Published user-facing intake → structured handoff packets
- **MAG-Self-Evolution-Monitor** — Continuous propose-not-execute evolution monitoring
- **MAG-PA-Flow-Engineer** — Checksum-gated Power Automate CreateFlow/UpdateFlow engineering child
- **MAG-Fleet-Architect** & **MAG-Fleet-Meta-Documenter** — Design advisory and meta-layer documentation

The architecture emphasizes source discipline, explicit handoff contracts (ChildResult, IntakeHandoffPacket, EvolutionProposalPacket, etc.), approval-gated writes, and self-test alignment.

### Document Intelligence & Parsing Pipelines
Python-centered pipelines that convert customer RFQs and technical specifications into structured, evidence-backed artifacts:
- Concise engineer briefs
- Canonical JSON / knowledge packs
- Source ledgers and evidence references
- Missing-input and conflict reports
- Operational run summaries

Emphasis remains on deterministic structure, provenance, and clean handoff to downstream agents or human reviewers (MAG-Auto-Parse methodology).

### Power Platform & Quote Workflow Automation
A suite of production Power Automate flows (SCA series) that connect Salesforce cases, SharePoint quote folders, Teams notifications, attachment handling, case-owner updates, and notebook generation. Additional governed tooling covers flow lifecycle, payload serialization guards, and inventory/registry management.

### Skills & Authoring Toolkits
Reusable Copilot Studio Skills (and the meta-toolkit that authors them) for:
- Skill, instruction, knowledge-source, and connected-agent description authoring
- Copy-ready output formatting
- Child-result integration, deliverable transport, Salesforce case source lookup, and more

These live in the fleet repos and are designed for reliable generative orchestration.

### Industrial Automation Domain
Support for engineered material-handling applications involving Magnetek drives and automation products, VFD motion control, HMI concepts, safety interlocks, diagnostics, and proposal generation for crane and hoist systems.

---

## Frameworks & Supporting Work

- **Event-Horizon IDEA** — Platform- and domain-neutral framework for building, governing, and evolving AI agent systems using the IDEA cycle (Innovate → Develop → Evaluate → Automate). Provides portable patterns, governance, agent archetypes, and handoff contracts.
- **agent-fleet-os** — Implementable platform-neutral OS (schemas, role archetypes, validators, pipelines, adapters for Copilot Studio / Grok / others). Magnetek RFQ is the reference domain adapter.
- **Grok + Copilot Studio integration patterns** — Documentation and guides for using xAI Grok alongside Microsoft Copilot Studio in industrial automation contexts.

---

## Tech Stack

**Core**  
Python · PowerShell · JSON Schema · Markdown · Structured output contracts · GitHub as source of truth

**Microsoft 365 / Power Platform**  
Copilot Studio · Power Automate · Power BI · Dataverse · SharePoint · Teams · Outlook · Loop

**AI & Document Intelligence**  
Multi-agent orchestration · Evidence-backed extraction · Prompt & instruction design · RFQ/spec parsing · Compliance matrix support · Multi-LLM experimentation (including Grok)

**Industrial Automation**  
PLC-based overhead crane motion control · Magnetek crane & hoist systems · VFD motion control · HMI & diagnostics · Safety interfaces · Engineered material-handling proposals

---

## Key Repositories

Most of the MAG work is private (internal Magnetek / CMCO use). Public-facing profile and supporting frameworks:

| Repository | Purpose |
|---|---|
| [hermansmpjr](https://github.com/hermansmpjr/hermansmpjr) | This profile |
| [MAG-Fleet](https://github.com/hermansmpjr/MAG-Fleet) | Production runtime — agent instructions, skills, routing, Power Automate inventory |
| [MAG-Fleet-Meta](https://github.com/hermansmpjr/MAG-Fleet-Meta) | Meta / control plane — Governor, Factory, Knowledge pipeline, governance, evolution |
| [MAG-FLEET-DEV](https://github.com/hermansmpjr/MAG-FLEET-DEV) | Staging / validation sandbox |
| [event-horizon](https://github.com/hermansmpjr/event-horizon) | IDEA cycle framework (platform- & domain-neutral) |
| [agent-fleet-os](https://github.com/hermansmpjr/agent-fleet-os) | Platform-neutral multi-agent OS (schemas, roles, validators) |
| [grok-copilot-studio-integration](https://github.com/hermansmpjr/grok-copilot-studio-integration) | Grok ↔ Copilot Studio integration patterns |

---

## Key Initiatives

- **Better Way Builders / I.D.E.A.** — Internal community and methodology for employee-led improvement, experimentation, documentation, and automation.
- **Governed Idea-to-Sustainment Workflow** — Structured path from concept through documentation, validation, controlled publication, and sustained operation (GitHub as canonical source, controlled SharePoint publication).
- **Self-Improving Multi-Agent Fleet** — Agents that can propose, generate, and evolve other agents under strong governance, source discipline, and approval gates.

---

> I'll gladly invest hours or days to save seconds or minutes, because those small gains compound over time. Time is the only resource we can never recover once it's spent.

---

**Connect**

- [LinkedIn](https://www.linkedin.com/in/michaelhermans) — Mike Hermans
