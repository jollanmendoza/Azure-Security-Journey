# Azure and GRC Learning Journey

## Certification Roadmap
- [ ] AZ-900: Azure Fundamentals (Target: January 2026)
- [ ] SC-900: Security, Compliance, and Identity (Target: February 2026)

## Daily Learning Log

### Day 1: Foundation & Infrastructure Setup
**Date:** December 30, 2025
**Focus:** Cloud Fundamentals & GRC Environment Setup

- [x] **Portfolio Infrastructure:** Created GitHub Repository `Azure-Security-Journey` and initialized documentation structure.
- [x] **GRC Tracking:** Configured Notion Database for AZ-900/SC-900 exam tracking and terminology management.
- [x] **Shared Responsibility Model:** Created a comprehensive responsibility matrix for IaaS, PaaS, and SaaS service models.
- [x] **Key Takeaway:** Understood that regardless of the cloud model, the consumer is always responsible for Data, Identities, and Devices.

**Files Created/Updated:**
- `README.md` (Progress Log)
- `cloud-fundamentals.md`
- `shared-responsibility.md`

### Day 2: Management Tools & Active Recall Systems
**Date:** January 12, 2026
**Focus:** Azure Interaction Methods & Active Recall Integration

- [x] **Active Recall System:** Within my Notion database, I created the "Active Recall: Responsibility Matrix" table. This table maps concepts across IaaS, PaaS, and SaaS to identify ownership (Consumer, Provider, or Shared).
- [x] **Glossary Infrastructure:** Within the same Notion database, I configured a second Notion Table for Terminology & Concept Tracking (Updated Version of Day 1 **GRC Tracking**). This includes:
  - **Service/Concept Name**
  - **Exam Tracking (AZ-900/SC-900)**
  - **Learning Status** (Mastered, In Progress, Not Started)
  - **GitHub Linkage:** Direct links back to the `Azure-Security-Journey` repository for integrated documentation.
- [x] **Interaction Mastery:** Documented the primary methods for interacting with Azure, specifically the Azure Portal (GUI) and the Command Line Interface (CLI).
- [x] **Key Takeaways:** Linking Notion status tracking directly to GitHub documentation creates a closed-loop learning system, ensuring no terminology gaps before exam day.

**Files Created/Updated:**
- `README.md` (Progress Log)
- `azure-architecture.md`

### Day 3: Physical Infrastructure & Resiliency
**Date:** January 16, 2026
**Focus:** Datacenters, Regions, and High Availability

- [x] **Physical Layer:** Documented the hierarchy of datacenters - availability zones - regions.
- [x] **Resiliency Planning:** Studied the "300 mile" rule of Region Pairs and how they ensure business continuity during large-scale disasters.
- [x] **GRC Integration:** Identified how region pairs maintain residency for legal and tax compliance with the same geography.
- [x] **Key Takeaways:** Availability zones protect against local (datacenters) failure, while region pairs protect against regional (geographic) disasters.

**Files Created/Updated:**
- `README.md` (Progress Log)
- `azure-architecture.md` (Added Physical Infrastructure Section)
- Notion: Added 5 new terms to Glossary and 3 to responsibility matrix.

### Day 4: Logical Infrastructure & Governance Hierarchy
**Date:** January 17, 2026
**Focus:** Resource Organization, Subscriptions, and Management Groups

- [x] **Hierarchy Mastery:** Documented the 4-level management hierarchy: **Management Groups → Subscriptions → Resource Groups → Resources.**
- [x] **Governance at Scale:** Explored how Management Groups allow for "Enterprise-grade" governance by applying conditions to 10,000+ groups in a single directory.
- [x] **Compliance Isolation:** Analyzed how to use separate subscriptions for **Environment Isolation** (Dev vs. Prod) to satisfy audit and compliance requirements.
- [x] **Key Takeaway:** Governance is inherited. Applying a security policy at the Management Group level ensures every resource below it is compliant by default.

**Files Created/Updated:**
- `README.md` (Progress Log)
- `azure-architecture.md` (Added Management Infrastructure Section)
- Notion: Added 5 new terms to Glossary and 3 to responsibility matrix.

### Day 5: Azure Management & Cloud Economics
**Date:** January 18, 2026 
**Focus:** Cost Factors, Billing Zones, and Marketplace Compliance

- [x] **Economics Transition:** Documented the shift from CapEx to OpEx and the factors influencing variable costs.
- [x] **Financial Governance:** Analyzed "Pay-as-you-go" vs. "Reserved Capacity" (1-3 year commitments) for cost optimization.
- [x] **Network Cost Modeling:** Defined the difference between Inbound (Free) and Outbound (Paid) data transfers across Billing Zones.
- [x] **Marketplace Integrity:** Noted that all 3rd-party solutions in the Azure Marketplace must be certified and compliant with Azure standards.
- [x] **Key Takeaway:** Geography isn't just about latency; it's about local tax, labor, and power costs which directly influence the resource price point.

**Files Created/Updated:**
- `README.md` (Progress Log)
- `azure-governance-and-compliance.md` (new file started)
-  Notion: Added 4 new terms and 2 recall questions.

### Day 6: Cost Management & Financial Governance
**Date:** January 19, 2026
**Focus:** Cost Estimation, Budgeting, and Financial Oversight

- [x] **Cost Estimation Mastery:** Documented the use of the **Azure Pricing Calculator** to forecast expenses for Compute, Storage, and Networking prior to deployment.
- [x] **Automated Governance:** Analyzed the three primary **Cost Alert** types:
    - **Budget Alerts:** Threshold-based notifications for usage/cost.
    - **Credit Alerts:** Specific for Enterprise Agreements (EA) monetary commitments.
    - **Department Quotas:** Email notifications for department-level spending thresholds.
- [x] **Key Takeaway:** Financial governance in Azure is proactive. Using calculators to plan and alerts to monitor ensures the OpEx model remains predictable and stays within organizational compliance boundaries.



**Files Created/Updated:**
- `README.md` (Progress Log)
- `azure-governance-and-compliance.md` (Completed the Financial Governance chapter)
- Notion: Added 5 new Glossary terms and 3 Active Recall questions focused on Cost Management.
