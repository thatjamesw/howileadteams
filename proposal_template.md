# Proposal Template  

A proposal is a lightweight artefact designed to **align stakeholders** on context, hypothesis, validation, and direction before a single line of code is written.  It promotes clarity, shared understanding and measurable outcomes while avoiding premature development or rework.  

---

## 1. Executive Summary  
Provide a concise overview of the problem, opportunity, and intent of the proposal.  

**Examples**  
- What is the issue or opportunity being addressed?  
- Why is this important now?  
- What is the desired outcome or success measure?  

Keep this section brief — two or three paragraphs that a senior stakeholder can read and immediately understand the value and direction.  

---

## 2. Stakeholders and Alignment  
List the key individuals or groups involved in this proposal. Clarify roles and responsibilities to ensure visibility and accountability.  

| Role | Name / Team | Responsibility |  
|------|--------------|----------------|  
| Sponsor |  | Provides approval and prioritisation |  
| Product Owner |  | Defines business goals and success criteria |  
| Technical Lead / Architect |  | Owns technical feasibility and design |  
| Delivery Lead / Scrum Master |  | Facilitates planning and execution |  
| Key Contributors |  | SMEs or supporting teams |  

---

## 3. Hypothesis and Validation

### 3.1 Hypothesis Statement
State your working hypothesis — what you *believe* to be true or achievable.  
This is your starting assumption that guides discovery and solution design.  

**Example Hypothesis Structure**  
> *We believe that by [doing X], we will achieve [Y outcome], measured by [Z metric].*  

The hypothesis sets direction but remains open to validation and iteration.  

### 3.2 Validation of Hypothesis  
Summarise the research, data, or early testing used to validate (or challenge) the hypothesis.  

**Consider including**  
- Data points or findings that support the proposal.  
- Risks, dependencies, or unknowns identified during exploration.  
- Input from workshops, user sessions, or peer review.  

This ensures the proposal is grounded in evidence rather than assumption.  

---

## 5. Requirements
Summarise what must be true for this proposal to succeed. Keep this focused and testable; detailed specs can live in linked epics/stories.

### 5.1 Functional Requirements (FRs)
Describe the user-visible behaviours and system capabilities.

| ID | Requirement | Rationale | Acceptance Criteria / Test Notes |
|----|-------------|-----------|----------------------------------|
| FR-01 |  |  |  |
| FR-02 |  |  |  |

> Tip Use MoSCoW where helpful (Must / Should / Could / Won’t).

### 5.2 Non-Functional Requirements (NFRs)
Quality attributes and guardrails. Prioritise the few that matter here; link to deeper standards if needed.

| Area | Requirement / Target | Measure / Evidence |
|------|----------------------|--------------------|
| Performance | e.g., p95 latency ≤ 300 ms under 2k RPS | Load test results |
| Availability | e.g., ≥ 99.9% monthly | SLO/SLA definition |
| Reliability / Resilience | e.g., graceful degradation, retries, backoff | Chaos test notes |
| Security | e.g., private endpoints only, managed identities | Threat model / policy refs |
| Privacy / Compliance | e.g., GDPR data minimisation | DPIA / data map |
| Cost | e.g., ≤ €X/month at baseline | Cost model / dashboard |
| Observability | e.g., traces + logs + SLO alerts | Runbook / dashboards |
| Scalability | e.g., horizontal scale to 3× baseline | Capacity plan |
| Operability / Support | e.g., runbooks, on-call, RTO/RPO | Docs / drills |
| Maintainability | e.g., IaC, linting, CI checks | Pipeline gates |

### 5.3 Constraints & Assumptions
Record anything that narrows options or must be true.

- **Constraints**
  - (e.g., must use Azure Bicep and ADO; data must reside in EU.)
- **Assumptions**
  - (e.g., Sweden region quota will be approved; existing VNets reused.)

### 5.4 Dependencies
List upstream/downstream teams, services, or decisions that affect delivery.

| Item | Owner / Team | Type (Tech/Process) | Needed By | Risk |
|------|--------------|---------------------|-----------|------|

### 5.5 Acceptance Criteria (Outcome-level)
Tie back to the Executive Summary and success measures.

- Metric-based outcomes (e.g., “reduce cycle time by 20% within 2 sprints”).
- Compliance gates (e.g., “all NFRs at Must level met; Should items have a plan”).

---

## 6. Solution Design  
Outline the proposed solution at a conceptual or architectural level.  
Include enough detail to explain the approach — without going into full implementation detail.  

**Recommended structure**  
- **Overview** Describe the solution direction and rationale.  
- **Key Components** Summarise major systems, integrations, or patterns.  
- **Alternatives Considered** Capture other options evaluated and why they were rejected.  
- **Risks and Mitigations** Highlight any concerns and how they can be addressed.  

Use diagrams or bullet points for clarity.  

---

## 7. Pros and Cons  
Provide a balanced assessment of the proposed approach.  

| Aspect | Pros | Cons |  
|---------|------|------|  
| Technical |  |  |  
| Business |  |  |  
| Operational |  |  |  
| Cost / Effort |  |  |  

This promotes transparent decision-making and helps stakeholders understand trade-offs.  

---

## 8. Cost and Impact Assessment  
Provide a high-level understanding of the cost implications and expected business impact.  
This section ensures decisions are made with both **technical** and **financial awareness**.  

**Suggested breakdown**  
- **Estimated Effort / Timeframe** e.g. 20–25 person-days or 3 sprints.  
- **Direct Costs** cloud consumption, licences, third-party tools, external consultancy, etc.  
- **Indirect Costs** training, operational overhead, process changes, or support.  
- **Potential Savings or Value** reduction in manual work, improved stability, time-to-market, or scalability.  
- **ROI Considerations** short-term vs. long-term benefits and payback period if relevant.  

Where possible, provide ranges or relative comparisons — precision is less important than transparency and shared understanding.  

---

## 9. Plan Forward  
Define the next steps and success checkpoints.  

**Include**  
- Recommended path forward (e.g. MVP, proof of concept, full implementation).  
- Key milestones and dependencies.  
- Definition of success and metrics to measure progress.  
- Decision points for future review or scaling.  

Keep the plan lightweight — the goal is alignment, not project planning.  

---

## 10. Approval and Review  
Document the sign-off or agreement from relevant stakeholders.  
Include dates and any follow-up review cycles.  

| Name | Role | Decision | Date | Comments |  
|------|------|-----------|------|-----------|  

---

## Example Usage  
The proposal template should be used before large or high-impact work begins.  

It helps the team:
- Align on *why* something is needed before deciding *how*.
- Design the solution 
- Engage stakeholders early, reducing risk of misalignment.
- Capture context that informs future development or retrospective review.

---

### Suggested File Naming  
Store proposals in your repo or shared space with a clear naming convention  
