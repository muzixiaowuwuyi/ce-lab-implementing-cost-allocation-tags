# Tagging Strategy

## Required Tags
1. **Environment:** production | staging | development
2. **Owner:** team-name or email
3. **Project:** project-identifier  
4. **CostCenter:** department code

## Tag Naming Conventions
- Keys: PascalCase (e.g., Environment, Owner, Project, CostCenter)
- Values: lowercase-with-dashes (e.g., development, data-ops-team, bootcamp, cloud-training-01)

## Enforcement
- **Detective Control:** AWS Config rule `required-tags` to monitor and audit resource compliance.
- **Preventative Control:** Future implementation of Infrastructure as Code (IaC) via Terraform using `default_tags` and AWS Organizations Tag Policies.