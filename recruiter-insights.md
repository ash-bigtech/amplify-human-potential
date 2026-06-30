# Recruiter Insights — Full Stack Engineer Pre-Qualification

**Internal use only — Humanoid Talent Team**

This document accompanies the candidate-facing pre-qualification form for the **Full Stack Engineer, Platform & Applications** role (London). It contains the recruiter insight for each question: what signal it's designed to surface, and how to interpret strong, weak, or ambiguous answers. Question numbers match the form exactly.

---

## Module A — Logistics & Core Eligibility

**01. Right to work in the UK**
Hard gate for compliance. Immediately determines sponsorship feasibility — route "requires sponsorship" candidates to a separate workflow rather than discarding; Humanoid may open sponsored tracks as headcount grows.

**02. Location & relocation**
Determines pipeline urgency. London-based candidates can start sooner. Relocation intent and timeline flag cost considerations early, avoiding offer-stage surprises.

**03. Onsite commitment**
Non-negotiable for this role — physical proximity to robot hardware is essential for the edge-device development loop. The nuance between "prefer" and "can commit" surfaces candidates who may eventually seek hybrid arrangements.

**04. Availability & notice period**
Sets pipeline sequencing. Flags whether a candidate can be "banked" for a later cohort. Lengthy notice periods are not disqualifying — they often signal seniority — but enable accurate offer-timing strategy.

---

## Module B — Technical Core & Stack Mastery

**05. Hands-on coding proficiency**
Self-ratings are a starting signal, not ground truth. Flag any candidate rating Rust or Golang at 4–5 — these are rare and valuable for edge-device services. The React / alternative framework split reveals whether UI experience is React-specific or genuinely framework-agnostic. Mismatches between stated scores and portfolio depth should surface in the technical screen. A pattern of all 5s with a thin GitHub is a red flag.

**06. Full-stack spectrum — where is your core anchored?**
This is a signal vector, not a filter. Humanoid needs backend-leaning or infrastructure-leaning engineers for the cloud and edge layers, but a balanced candidate may be the team's connective tissue.

**07. Digital footprint & portfolio links**
GitHub activity — pinned repositories, commit cadence, language distribution — should be reviewed before the technical screen. Google Scholar is particularly relevant if the candidate has robotics, ML systems, or distributed computing research. A strong Stack Overflow profile signals community engagement and communication clarity.

---

## Module C — Advanced Infrastructure, SDLC & Scale

**09. Infrastructure as Code & platform ownership**
The centralised robot fleet platform will demand deep IaC ownership — not just "I've used Terraform." Look for candidates who can describe trade-offs between tools (e.g. Pulumi vs Terraform when dealing with dynamic configuration), and who have owned Kubernetes in production, not just in development. Kubernetes experience at the edge (k3s, microk8s) is a strong differentiator for this role.

**08. SDLC evolution — from prototype to production** *(optional question)*
The HMND 01 platform will go through exactly these three phases at speed. Look for candidates who can articulate the specific technical and organisational challenges at each phase transition — not just those who have "shipped to production." Answers that skip the pilot phase or conflate POC with production suggest limited experience with deployment at scale.

---

## Module D — Data Privacy, Compliance & Security

**11. Data governance & edge-to-cloud privacy practice**
Humanoid's data handling will face significant regulatory scrutiny, particularly around video and spatial data captured in shared workspaces. Candidates who have built consent management, data minimisation pipelines, or per-tenant data isolation in prior roles carry disproportionate value. Distinguish between "we had a DPO handle compliance" and "I designed the data flow to be GDPR-compliant by construction" — the latter is the stronger signal.

**10. Telemetry, observability & distributed system health** *(optional question)*
This is the single deepest technical filter in the form. Robot fleet telemetry at scale is a genuinely hard distributed systems problem. Strong answers will mention specific protocol trade-offs (MQTT vs gRPC for constrained hardware), edge buffering strategies for intermittent connectivity, and structured log design. Candidates who only mention "I've used Datadog" have not solved this problem at the relevant depth.

---

## Module E — Culture, Velocity & Financial Alignment

**12. Company-stage experience & environment fit**
Candidates who have only worked in mature organisations with established engineering cultures will often struggle in Humanoid's environment — not because they lack technical skill, but because the operating model is fundamentally different. Early-stage or deep-tech startup backgrounds are high-fit proxies. The comfort question quickly surfaces misalignment without requiring a lengthy written answer.

**13. Compensation & financial alignment**
Equity context is critical — a candidate sitting on £200k+ unvested equity at a late-stage company is a structurally different conversation than one who is fully liquid. Understanding the full compensation picture enables Humanoid to construct a compelling offer, particularly where cash compensation may not match FAANG-level salaries but equity upside in a robotics platform is significant. Do not skip this section or treat it as optional.

---

*This document should not be shared with candidates or external parties.*
