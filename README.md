# TCS-AI-Friday-usecase
TCS AI Friday usecase
User Story 
AI Powered Personalized Onboarding Assistant (Employee 306090 Day Copilot) 
Personalized, Role Aware Onboarding to Replace Generic “Information Dump” 
New hires want a personal onboarding guide that delivers role specific tasks, training, and 
connections at the right time—so they can ramp up quickly without information overload. HR 
and hiring managers want onboarding to be consistent, measurable, and low touch, with 
automation for scheduling, training assignment, and answering repetitive questions. 
Objective 
• Generate a dynamic onboarding plan (Day1 → Day90) personalized by:  
o Role, department, seniority/level, location, joining date, manager/team 
context 
• Provide a conversational assistant that answers onboarding FAQs using a curated 
knowledge base. 
• Prevent overload via dripfeed delivery: tasks and information appear when needed 
(context + timeline based). 
• Demonstrate two different job roles with visibly different tasks, training, and 
recommended connections. 
• Integrate with:  
o Calendar to auto-schedule introductory meetings 
o LMS to assign relevant trainings and track completion 
• Enforce governance: identity, RBAC, audit logs, privacy-by-design, and human 
override. 
Expected Outcomes 
• Higher new hire engagement & satisfaction → improved retention 
• Faster time to productivity via role-specific enablement 
• Reduced HR and manager administrative burden 
• Improved compliance completion rates and visibility 
• Stronger culture/belonging through guided connections 
Deliverables (Either Option 1a & 1b OR Option 2) 
All deliverables are expected to be production-level quality, ensuring excellence in both 
content and look & feel. 
Option 1a: “Onboarding Journey Advisor” (AI Assistant) 
A conversational assistant that: 
• Creates a personalized 306090 plan 
• Answers FAQs with citations to onboarding policy sources 
• Proactively recommends “Today’s Top 3” tasks 
• Tracks completion, nudges gently, escalates blockers (e.g., access pending) 
Option 1b: Onboarding Dashboard (HR + Manager View) 
A dashboard that shows: 
• Cohort-wise and individual progress 
• Compliance training completion status 
• Access/tool enablement status (pending approvals) 
• Engagement signals (assistant usage, unresolved questions) 
• Bottlenecks & SLA (ticket aging, approvals pending) 
Option 2: End-to-end “Mock” Personalized Onboarding Flow (Agentic Lite) 
A simulated flow demonstrating: 
• New hire profile created from HR feed  
•  AI generates personalized onboarding plan  
• Meetings auto scheduled via Calendar  
• Training assigned via LMS  
• Assistant answers questions + nudges progress  
• Tickets created automatically for blockers  
• Evidence & audit trail generated 
Supported Request Types 
Choose either “always-on assistant” or implement one or more below: 
1. Day1 Setup & Logistics  
o laptop shipping, badge, VPN, email, Teams setup 
2. Access & Tools Enablement  
o repo, cloud subscription, CRM, BI tools, shared drives 
3. Policy & Compliance  
o security, privacy, code of conduct, travel policy 
4. Role Enablement  
o engineering SDLC, marketing playbook, sales process, etc. 
5. People & Culture  
o buddy connect, team introductions, communities/ERGs 
6. First Deliverables  
o first sprint task, first campaign brief, shadowing sessions 
7. FAQ / Q&A  
o benefits, payroll, leave, reimbursement, internal portals 
Core Functional Scope (Choose based on the deliverable) 
1. New Hire Profile Intake 
Inputs (synthetic for demo): 
• Role, department, location, level, start date, manager, team 
• Onboarding templates by role (config) 
• Location rules (office, holidays/time zones, local compliance) 
Outputs: 
• Personalized plan parameters + recommended connections + training bundle 
2. Dynamic 306090 Plan Generator 
Plan sections 
• Day 0–7: essentials + access + culture basics 
• Week 2–4: role foundations + first output 
• Day 30–60: deeper ownership + cross-team working 
• Day 60–90: autonomy milestone + measurable impact 
Personalization logic 
• Level increases complexity and stakeholder mapping 
• Role changes training modules & early deliverables 
• Location changes logistics, local policies, office onboarding 
3. Knowledge Base Q&A (RAG-ready) 
• Curated onboarding content:  
o HR handbook, IT setup guides, tool FAQs, role playbooks 
• Conversational features:  
o intent detection (HR vs IT vs role enablement) 
o structured answers + citations/links 
o “Open a ticket” if not solvable via KB 
4. Drip-feed + Nudges Engine 
• Nudges based on:  
o day in journey (Day 1/Week 2/Day 30) 
o completion status (pending tasks) 
o dependencies (access pending → remind + escalate) 
• Examples:  
o “Complete Security Training by Friday” 
o “Schedule 1:1 with Manager” 
o “Your Git access request is pending—want me to follow up?” 
5. Calendar Integration 
Auto-create meetings: 
• Manager intro (Day 1) 
• Buddy connect (Day 2) 
• Team intro (Week 1) 
• Role-specific stakeholder meetings (Week 2–4) 
• 306090 review checkpoints 
6. LMS Integration 
• Assign mandatory modules:  
o security awareness, privacy, compliance 
• Assign role-based modules:  
o engineering: SDLC, CI/CD, repo practices, runbooks 
o marketing: brand, campaign lifecycle, tools 
• Track completion → nudges → manager escalation if overdue 
7. Progress Tracking & Reporting 
• New hire view:  
o timeline, checklist, “Today’s tasks,” upcoming meetings/training 
• HR/Manager view:  
o completion, bottlenecks, SLA tracking, satisfaction pulse 
Two-Role Demo Requirement (Must-Have) 
You must demonstrate two distinct journeys (tasks, trainings, connections differ). 
Role A Example: Software Engineer 
Week 1 
• Setup dev environment + repo access + secrets vault access 
• Complete security + privacy training 
• Meet: manager, buddy, tech lead Week 2–4 
• SDLC + CI/CD training 
• First sprint story; code review walkthrough Day 30–60 
• Own a small component; on-call orientation Day 60–90 
• Deliver feature end-to-end; contribute runbook/KB article 
Role B Example: Marketing Manager 
Week 1 
• Access: brand assets, marketing automation platform, CRM views 
• Brand guidelines + compliance training 
• Meet: manager, buddy, sales partner, product partner Week 2–4 
• Campaign process training; build first campaign brief Day 30–60 
• Run a pilot campaign with analytics dashboard Day 60–90 
• Own a quarterly campaign plan; present outcomes 
Required Tools & Environment (Reference Implementation Mapping) 
Identity Platform 
• Microsoft Entra ID (or Google Cloud Identity) for authentication & RBAC 
Conversational AI Platform 
• Microsoft Bot Framework (or Dialog flow / ServiceNow AI Studio) 
LLM 
• GPT4 class model (or Gemini equivalent) via enterprise endpoint 
Backend 
• Fast API or Node.js 
• Orchestrates: plan generation, policy checks, integrations, audit logs 
Frontend 
• React / Vue / Stream lit 
• Channels: Microsoft Teams, Slack, and/or web portal 
Database 
• PostgreSQL / Fire store 
• Stores:  
o user profile 
o plan timeline + tasks 
o completion states 
o conversation history (minimal) 
o audit logs + feedback signals 
Integrations 
• Calendar (Microsoft Graph / Google Calendar API) 
• LMS (API-based assignment + completion) 
• HRIS (mock feed for hackathon) 
KPIs & Success Metrics 
Experience & Productivity 
• Time-to-first-deliverable (proxy) 
• New hire satisfaction pulse score 
• Assistant adoption (DAU in first 30 days) 
Efficiency 
• HR/Manager time saved (ticket reduction) 
• Self-service resolution rate (% answered without human) 
• Median time to resolve onboarding blockers 
Compliance 
• Mandatory training completion SLA 
• % onboarding tasks completed by Day 7 / 30 / 90 
Instructions 
• Use synthetic data only 
• No real employee PII 
• Must demonstrate:  
o two roles with different journeys 
o calendar scheduling integration (real or simulated) 
o LMS assignment + tracking (real or simulated) 
o knowledge base Q&A with citations 
Quality Standards 
• Production-quality UI/UX (journey timeline + today’s tasks + status) 
• Guard railed LLM outputs:  
o policy questions grounded in KB 
o escalation paths when uncertain 
• Test cases:  
o personalization logic correctness 
o access control enforcement 
o scheduling correctness 
o training assignment and reminders 
Guardrails 
• RBAC: show only relevant content per role/location 
• Hallucination control:  
o cite KB sources; otherwise say “not found” + create HR/IT task 
• Privacy-by-design:  
o minimal employee profile data 
o secure storage; retention policy for chat logs 
• Human override for:  
o sensitive HR topics, exceptions, access escalations







User Story 
AI Led Real-time FinOps & Autonomous Cloud Cost Governance 
Finance, Cloud Ops, and Product/Engineering teams want an AI led FinOps system that can 
continuously monitor multi cloud spend, detect cost spikes and anomalies in near real 
time, identify the true cost drivers, recommend and (where policy allows) execute corrective 
actions automatically, and ensure budget adherence and governance without heavy manual 
analysis—delivering predictable spend, higher utilization efficiency, and faster value realization. 
Objective 
• Provide real-time visibility into cloud spend across multi cloud (Azure/AWS/GCP) with 
consistent tagging and allocation. 
• Detect cost anomalies early and explain drivers using AI (services, regions, 
subscriptions/projects, teams, workloads). 
• Enable predictive forecasting (daily/weekly/monthly) with “spend at risk” warnings. 
• Automate cost optimization actions (rightsizing, schedule off-hours, storage tiering, 
reserved/savings planning) using policy-driven autonomy. 
• Establish autonomous cost governance:  
o Budget guardrails, approval workflows, and exception handling 
o Evidence trails and audit readiness 
• Reduce manual FinOps effort through intelligent triage, summarized insights, and agent
driven remediation. 
Expected Outcomes 
• Reduce cost spikes and shorten time-to-diagnosis (MTTD) and time-to-remediation 
(MTTR) for anomalies 
• Prevent budget overruns through predictive + policy-driven controls 
• Improve resource utilization and reduce idle/overprovisioned services 
• Improve cost transparency via ownership mapping and unit economics 
• Increase FinOps maturity: from reporting → optimization → governance automation 
Deliverables 
All deliverables are expected to be of production-level quality, ensuring excellence in both 
content and look & feel. 
a. FinOps Optimization & Governance Dashboard (Visual Impact) 
A dashboard that provides: 
• Spend Overview (MTD, forecast EOM, variance vs budget) 
• Cost Spike Detector (hourly/daily anomalies, top impacted services) 
• Optimization Opportunities (rightsizing, idle resources, storage tiering, commitments) 
• Governance & Compliance (tag compliance, policy violations, exceptions) 
• Unit Economics (cost per product / environment / team / transaction) 
• Value Realization (savings achieved, avoided cost, reclaimed capacity) 
b. End-to-end “Mock” Autonomous FinOps Flow (Agentic Lite) 
A simulated E2E flow demonstrating: 
• Cost spike detected (real time alert from usage feed) 
• ITSM ticket auto-created (incident/problem/change based on severity) 
o An AI assistant that evaluates cost + usage + context and outputs: 
▪ Anomaly / Risk Score (spike severity, budget breach likelihood) 
▪ Root cause explanation (what changed, where, who owns it, why now) 
▪ Top drivers (service, SKU, tag, region, subscription/project, workload) 
▪ Recommendations (prioritized by impact and risk):  
▪ rightsizing, scaling policy updates, scheduling, storage lifecycle, 
reserved/savings plan 
▪ tagging fixes, allocation improvements, policy enforcement 
▪ Recommendation: Auto approve / Defer / Escalate / Execute (guard 
railed) / Rollback 
• Execution simulated:  
o stop idle resources, schedule non-prod shutdown, resize instances, delete 
orphan disks/snapshots, move storage to cool tier 
• Validation:  
o spend stabilizes 
o utilization improves 
o no SLA impact 
o rollback if negative impact 
• Ticket auto updated and closed 
• Dashboard shows anomaly → action → savings → evidence trail 
Suggested inputs (synthetic/public sample data only): 
• Cost & usage exports (daily/hourly) 
• Resource inventory + tags (owner/cost centre/environment) 
• Budgets, alerts, policy definitions 
• Deployment/change signals (CI/CD events, scale events—synthetic) 
• Ticket history (ITSM/FinOps tasks—synthetic) 
Supported Request Types 
Choose either always-on FinOps governance OR one or more categories below. 
FinOps Request Categories 
1. Cost Spike / Anomaly Investigation  
o “Why did spend increase 30% yesterday?” 
2. Budget Breach Prevention  
o “Forecast shows overrun—what actions to stay under budget?” 
3. Idle & Over Provisioned Resource Optimization  
o orphan disks, underutilized VMs, oversized databases, idle clusters 
4. Commitment Planning  
o Reserved Instances / Savings Plans / Committed Use Discounts 
5. Storage Cost Optimization  
o lifecycle tiering, snapshots cleanup, log retention optimization 
6. Tagging & Chargeback/Show back Governance  
o missing tags, ownership mapping, allocation rules 
7. Policy & Guardrail Enforcement  
o prevent expensive SKUs, region restrictions, environment scheduling policies 
8. Cost Allocation & Unit Economics  
o cost per customer, per app, per transaction 
Core Functional Scope (Choose based on deliverable) 
1. Data Ingestion & Normalization 
Sources 
• Cloud billing exports (Azure Cost Management, AWS CUR, GCP Billing export) (synthetic 
for demo if required) 
• Resource inventory & utilization metrics (CPU, memory, network, IOPS) 
• Tags/labels, account/subscription/project mapping 
• Budgets and forecast baselines 
Normalization 
• Common schema across clouds (service, SKU, region, owner, environment) 
• Tag quality scoring and enrichment (infer owner from org mapping if missing) 
2. Cost Observability (Real-Time Visibility) 
• MTD spend, daily/hourly trend 
• Spend by:  
o cloud → account/subscription → service → SKU → resource 
• Cost allocation views:  
o BU/team/app/environment 
• Variance analysis vs baseline 
3. Anomaly Detection & Root Cause Analysis 
Anomaly detection 
• Detect spikes against:  
o historical baseline, seasonality, deployment events, usage patterns 
• Severity classification:  
o Critical / High / Medium / Low based on $ impact + budget risk + business 
criticality 
RCA 
• Identify:  
o top services/SKUs contributing to delta 
o the “change point” (time and trigger) 
o correlated infra events (scale-up, new cluster, data transfer surge) 
• Explainable narrative:  
o “Spend increased due to 3 new GPU nodes in Region X deployed by Team Y for 
Project Z” 
4. Optimization Recommendation Engine 
Opportunity identification 
• Rightsizing recommendations 
• Idle detection and shutdown scheduling 
• Autoscaling policy tuning 
• Storage tiering and lifecycle policies 
• Network egress optimization (architectural hints) 
• Commitment planning (RI/Savings) based on steady-state usage 
• Database optimization (where relevant to cost) 
Prioritization 
• Impact ($) vs risk (SLA / performance) 
• Time-to-value 
• Effort complexity score 
5. Autonomous Remediation (Policy-Driven) 
Actions 
• Auto-stop non-prod workloads outside business hours 
• Delete orphaned disks / unattached IPs / stale snapshots 
• Resize underutilized instances (non-prod first) 
• Apply lifecycle policies to storage buckets/logs 
• Enforce tagging and quarantine non-compliant resources 
Control model 
• Safe-to-automate (no human approval) 
• Human-in-the-loop (approval required) 
• Prohibited (never auto-execute; only recommend) 
Rollback 
• Re-enable resource, revert size, restore snapshot (simulated for demo) 
6. Governance, Policy, and Compliance 
• Budget policies:  
o budget thresholds, EOM forecast breach rules 
• Controls:  
o allowed SKUs, region restrictions, max sizes for non-prod 
• Tag compliance:  
o required tags, ownership enforcement, exception expiry 
• Audit trail:  
o who asked, what was changed, why, before/after cost impact 
7. Tracking, Validation & Reporting 
Validation 
• Confirm cost reduction (before/after delta) 
• Ensure no SLA degradation (synthetic “SLO health” signals) 
• Monitor recurrence prevention (policy applied) 
Reporting 
• Weekly/monthly savings report 
• Executive scorecard:  
o budget adherence, optimization value, anomalies prevented, governance 
compliance 
• Backlog of opportunities and completed actions with evidence 
Dashboard (Sample Layout – What Users See) 
Top Strip (KPIs) 
• MTD Spend | Forecast EOM | Variance vs Budget | Anomalies (24h) | Savings 
Achieved (MTD) 
Panels 
1. Cost Spike Timeline (Hourly) 
2. Top Cost Drivers (Service/SKU/Region) 
3. Optimization Opportunities (Ranked) 
4. Idle/Overprovisioned Resources (Count + $) 
5. Governance Compliance (Tagging, Policy Violations, Exceptions) 
6. Unit Economics (Cost per Team/App/Env) 
KPIs & Success Metrics 
FinOps Outcomes 
• % reduction in idle spend 
• Cost spike MTTD / MTTR 
• Budget adherence rate 
• Savings achieved vs target (validated) 
• Forecast accuracy 
Governance Outcomes 
• Tag compliance % 
• Policy violations reduced 
• Exception closure rate / expiry adherence 
Operational Outcomes 
• Automation coverage (% actions auto-executed under policy) 
• Rework reduction (fewer manual investigations) 
Instructions 
• Use synthetic or public sample data only. 
• Do not include confidential customer billing or resource details. 
• Demonstrate:  
o anomaly detection + RCA 
o at least one autonomous action under guardrails 
o dashboard showing savings + evidence trail 
Quality Standards 
• Production-quality UX and insights narrative 
• Explainable AI outputs (traceable to data) 
• Secure integration pattern (least privilege) 
• Test cases:  
o anomaly detection accuracy 
o action safety & rollback 
o permission enforcement and audit logs 
• Clear documentation:  
o architecture, data schema, policy model, evaluation approach 
Guardrails 
• Strict RBAC and approval workflows for high-risk actions 
• Mandatory evidence and “reason for change” 
• Prevent actions that can impact production SLAs unless explicitly approved 
• Rollback strategy for every automated change 
• Drift detection to ensure policies stay enforced











User Story 
AI-Led E2E Intelligent Storage Management for Hybrid Data Infrastructure 
Storage, Platform, and Cloud Ops teams want an AI-led autonomous storage management 
capability that can discover, monitor, predict, optimize, and remediate storage issues across 
on-prem, hybrid, and cloud—including SAN/NAS/Object, Kubernetes persistent volumes, 
backup/replication systems, and high-performance storage tiers for AI/ML workloads—
with minimal manual intervention. The system should self-optimize performance, prevent 
capacity incidents, automate data lifecycle/tiering, ensure data protection & compliance, 
and provide an explainable trust layer (why it took an action, what data it used, and what 
impact it achieved). 
Objective 
• Establish always-on storage observability + intelligence across the enterprise storage 
estate. 
• Enable predictive capacity and performance governance (forecasting, anomaly 
detection, early warning). 
• Deliver autonomous optimization:  
o right-sizing, tiering, caching policies, QoS controls 
o automated cleanup (orphans, stale snapshots, unused volumes) 
o data lifecycle policies (hot → cool → archive) 
• Improve data protection posture:  
o backup success, replication health, immutable snapshots, RPO/RTO 
compliance 
• Support AI/ML workloads with performance guarantees:  
o high throughput, low latency, parallel IO patterns, GPU pipeline readiness 
• Provide policy-driven automation with guardrails:  
o safe-to-automate vs approval required vs prohibited 
o rollback readiness and evidence-based validation 
Expected Outcomes 
• Reduced incidents (capacity/performance failures) and faster MTTR through self
healing 
• Predictable capacity with time-to-exhaust forecasting and automated remediation 
• Lower storage spend through tiering, reclamation, and utilization improvements 
• Higher SLA compliance (latency, throughput, RPO/RTO) 
• Improved audit readiness with immutable logs, evidence packs, and policy 
compliance tracking 
Deliverables 
All deliverables are expected to be of production-level quality, ensuring excellence in both 
content and look & feel. 
a. Intelligent Storage Operations Dashboard (Visual Impact) 
A live dashboard that: 
• Shows fleet health (Green/Amber/Red) across all storage platforms 
• Highlights top risks (time-to-exhaust, hotspots, RPO breach risk, failure probability) 
• Shows workload profiles (AI/ML, analytics, transactional, general purpose) 
• Tracks optimization actions and validated savings/performance improvements 
• Provides governance views:  
o policy compliance (encryption, retention, immutability) 
o exceptions & approval queue 
o audit evidence pack readiness 
b. End-to-End “Mock” Autonomous Storage Ops Flow (Agentic Lite) 
A simulated E2E flow demonstrating: 
1. Signal detected: capacity forecast breach / latency spike / backup failure / replication 
lag 
2. Ticket auto-created (ITSM incident/change/request – simulated) 
3. AI diagnoses + approves safe action under policy 
An AI assistant that evaluates storage telemetry + workload context and outputs: 
• Risk score across dimensions:  
o capacity exhaustion risk 
o performance degradation risk 
o protection gap risk (backup/replication/RPO) 
o compliance risk (encryption, retention, immutability) 
• Root cause hypotheses (why the issue is happening)  
o noisy neighbour / hotspot volumes 
o IO saturation / queue depth anomalies 
o mis-tiered datasets 
o replication lag due to bandwidth contention 
• Optimization recommendations (ranked by impact vs risk) 
• Recommendation: Auto-execute (policy-safe) / Defer / Escalate / Rollback 
4. Execution simulated:  
o lifecycle tiering / cache policy adjustment / QoS enforcement 
o expansion or reclamation cleanup 
o snapshot remediation / replication bandwidth shaping 
5. Validation:  
o latency normalized, headroom restored, RPO back in compliance 
6. Ticket auto-updated and closed with evidence (before/after metrics, timestamps, 
decision log) 
7. GUI shows: health → action → impact → trust layer → rollback 
Suggested inputs (synthetic/public sample data only): 
• storage inventory (arrays, shares, volumes, buckets, PVs) 
• performance metrics (IOPS, latency, throughput, queue depth, cache hit ratio) 
• capacity metrics (used%, growth rate, forecast) 
• protection posture (backup status, replication lag, snapshot success) 
• cost signals (tier costs, $/GB, egress, storage class pricing—synthetic) 
• workload metadata (criticality, environment, maintenance window) 
Supported Request Types 
Choose either continuous autonomous storage governance OR one of the categories below: 
Storage Request Categories 
1. Predictive Capacity Management  
o time-to-exhaust forecasting, auto headroom provisioning 
2. Performance Optimization  
o latency/IOPS hotspots, QoS controls, cache/tiering tuning 
3. Data Lifecycle & Tiering  
o hot/cool/archive policies, dataset classification-based placement 
4. AI/ML Workload Enablement  
o high-throughput datasets, GPU pipeline staging, parallel IO tuning 
5. Backup/Snapshot/Replication Remediation  
o backup failures, replication lag, missed snapshots, RPO breaches 
6. Cost Optimization & Reclamation  
o delete orphans, stale snapshots, unused volumes; storage class optimization 
7. Compliance & Governance  
o encryption/immutability/retention, WORM, audit evidence generation 
8. Exception / Waiver Requests  
o temporary policy exemptions, legal hold, retention override 
Core Functional Scope (Choose based on the deliverable) 
1. Discovery & Inventory (Foundation) 
• Auto-discover assets:  
o arrays, controllers, shares, volumes, buckets, PVs, backup targets 
• Maintain authoritative inventory:  
o ownership, tags, workload mapping, environment classification 
• CMDB synchronization (simulated):  
o storage asset → app/service association 
2. Observability & Telemetry Collection 
• Continuous metrics ingestion:  
o IOPS, latency, throughput, queue depth, cache hit ratio 
o capacity utilization, growth rate, dedupe/compression ratio 
o health events (disk/controller alerts), error rates 
• Protection metrics:  
o backup success, snapshot schedules, replication lag, RPO compliance 
3. AI/ML Intelligence Layer 
Anomaly Detection 
• Detect spikes and abnormal patterns:  
o sudden latency increase 
o abnormal growth 
o backup failure clusters 
Forecasting 
• Predict:  
o time-to-exhaust (per volume/array/tier) 
o failure probability / risk window 
o expected performance degradation if trend continues 
Root Cause & Impact Analysis 
• Identify:  
o top talkers (volumes/buckets/PVs) 
o noisy neighbour effects 
o misplacement across tiers 
o bandwidth contention affecting replication/backup 
• Estimate blast radius:  
o which applications and SLAs are at risk 
4. Policy & Guardrails (Autonomous Governance) 
• Define guardrails:  
o safe-to-automate actions (no approval) 
o approval required actions 
o prohibited actions (never auto) 
• Enforce constraints:  
o maintenance windows 
o data residency/retention rules 
o encryption and immutability mandates 
• Approval routing:  
o storage admin / app owner / security / compliance (as required) 
5. Autonomous Optimization & Remediation 
Typical Actions (simulated for demo) 
• Capacity:  
o reclamation cleanup, archive old data, expand volume, rebalance pools 
• Performance:  
o QoS adjustment, tier promotion for hot datasets, cache policy tuning 
• Protection:  
o rerun failed backups, reschedule snapshot jobs, throttle heavy jobs during 
backup windows 
o adjust replication bandwidth or reseed replication 
Self-Healing 
• Retry with diagnostics for transient errors 
• Escalate if repeated failures occur 
Rollback 
• Snapshot before change 
• Revert policies/QoS/tiering if validation fails 
6. Validation & Evidence 
• Compare before/after metrics:  
o latency p95/p99, IOPS, throughput 
o capacity headroom improvement 
o backup success restored, replication lag reduced 
• SLA confirmation:  
o ensure no performance regression 
• Evidence pack generation:  
o decision log, approvals, action trace, metrics proof, timestamps 
7. Reporting & Continuous Improvement 
• Executive scorecard:  
o incidents prevented, cost savings, compliance posture, automation coverage 
• Operational scorecard:  
o top recurring hotspots, time-to-remediate, action success rate 
• Feedback loop:  
o accept/reject AI recommendations and learn patterns 
Dashboards (Sample Panels & KPIs) 
Top KPI Strip 
• Fleet Health | Time-to-Exhaust (Critical Assets) | Hotspots (24h) | RPO Breaches | 
Savings Achieved (MTD) | Automation Coverage 
Core Panels 
1. Capacity Forecast & Risk Heatmap  
o volumes/tiers with < 7 / 30 / 60 days to exhaust 
2. Performance Hotspot Analyzer  
o top latency contributors and IO contention map 
3. AI/ML Workload Readiness  
o high-throughput datasets, staging tier health, GPU pipeline IO profile 
4. Protection Posture  
o backup/snapshot success, replication lag, RPO/RTO compliance 
5. Optimization Actions  
o recommended vs executed, impact realized, rollback events 
6. Governance & Compliance  
o encryption/immutability/retention compliance %, exceptions, approvals 
pending 
KPIs & Success Metrics 
Operational 
• Capacity incidents avoided 
• Performance incident reduction 
• MTTR reduction (from detection to stabilization) 
Financial 
• % idle storage reclaimed 
• cost savings via tiering and cleanup 
• utilization improvement (used vs provisioned) 
Reliability & Protection 
• backup success rate 
• replication lag reduction 
• RPO/RTO compliance rate 
Automation & Governance 
• % actions auto-executed safely 
• approval cycle time for high-risk actions 
• audit evidence completeness score 
Instructions 
• Use synthetic or public sample data only 
• Do not include confidential or customer storage information 
• Demonstrate at least:  
o one predictive insight (forecast/anomaly) 
o one optimization action (safe-to-automate) + validation 
o trust layer and audit/evidence trail 
Quality Standards 
• Production-quality UX (dashboard + conversational assistant) 
• Explainable AI outputs (what data drove the decision) 
• Policy-driven autonomy with clear guardrails 
• Functional + non-functional tests:  
o performance, resilience, security, rollback safety 
• Clear documentation:  
o architecture, data model, policy matrix, test cases, demo walkthrough 
Guardrails 
• Never auto-execute destructive actions without approval (delete, retention reduction, 
permanent tier change) 
• Snapshot-before-change for reversible actions 
• Permission controls and audit logs for every action 
• Data protection first: enforce immutability/retention policies where applicable 
• Hallucination control:  
o recommendations must be grounded in observed telemetry + policy 
 
