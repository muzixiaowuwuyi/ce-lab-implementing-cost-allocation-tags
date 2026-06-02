# AWS Cost Visibility & Governance Lab

## 📌 Project Overview
This project demonstrates the implementation of a robust **Cloud Governance and FinOps (Financial Operations) framework** on AWS. The core objective is to move from zero cost tracking to granular visibility by establishing a strict tag taxonomy, activating cost allocation tracking, and setting up automated compliance auditing.

This hands-on lab reflects standard production-grade DataOps/DevOps environment preparation where tracking infrastructure spend by environment, team, and project is legally and financially required.

## 🛠️ Implemented Architecture & Workflow
1. **Tag Taxonomy Design:** Defined an organization-wide standard using PascalCase for Keys and lowercase-with-dashes for Values across 4 core pillars (`Environment`, `Owner`, `Project`, `CostCenter`).
2. **Bulk Remediation:** Leveraged **AWS Tag Editor** to apply consistent tags across multiple distributed infrastructure resources (EC2, S3).
3. **FinOps Activation:** Activated user-defined cost allocation tags within the AWS Billing Console to initiate resource-level cost tracking for Cost Explorer.
4. **Automated Auditing (Detective Control):** Configured an **AWS Config Managed Rule** (`required-tags`) to continuously scan, monitor, and report non-compliant resources.

## 📁 Repository Structure
```text
.
├── tagging-strategy.md         # Corporate tagging policies and conventions (Step 1)
├── tag-compliance-report.md    # Audit results, KPIs, and remediation strategies (Step 6)
├── README.md                   # Project documentation (This file)
└── screenshots/                # Evidence of cloud infrastructure alignment
    ├── config-compliance.png   # AWS Config dashboard showing resource audit