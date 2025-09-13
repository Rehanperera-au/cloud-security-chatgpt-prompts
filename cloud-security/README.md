# Cloud Security Prompts

This section collects curated ChatGPT prompts specifically related to cloud security. Use these templates to help identify misconfigurations, evaluate security posture, and guide remediation across AWS, Azure, GCP, and multi‑cloud environments.

## Guidelines

- Only include prompts that are directly relevant to cloud security (e.g. infrastructure as code reviews, CSPM analyses, threat modelling).
- Avoid generic or unrelated prompts.
- Keep prompts short, focused, and actionable.
- Where possible, reference specific cloud services (e.g. S3, EC2, IAM policies, Azure storage accounts) or industry best practices.

## Example Prompts

- **Terraform review:** "You are a cloud security analyst. Review the following Terraform configuration and point out any security misconfigurations or missing best practices. For each finding, explain the risk and suggest a fix:\n\n```
<PASTE TERRAFORM HERE>
```"
- **S3 bucket policy:** "Analyse the following AWS S3 bucket policy. Identify any statements that make the bucket public or overly permissive and propose a secure alternative:\n\n```
<POLICY JSON>
```"
- **Kubernetes RBAC audit:** "Given the following Kubernetes Role and RoleBinding definitions, evaluate whether least privilege is enforced. Highlight any dangerous permissions and recommend stricter RBAC rules:\n\n```
<YAML MANIFEST>
```"
- **Azure storage encryption:** "Review this Azure Storage Account configuration JSON and determine if encryption at rest and TLS/HTTPS settings meet best practices. If not, explain why and suggest improvements."

## Wiz CSPM Prompts

If you use the Wiz cloud security posture management platform, these prompts can help interpret and act on Wiz findings:

- **Summarise Wiz Findings:** "Act as a cloud security consultant. Given the following list of Wiz CSPM findings, group them by severity and service, summarise the top risks, and recommend prioritised remediation steps:\n\n```
<WIZ FINDINGS>
```"
- **Investigate a finding:** "You are a security engineer. Interpret the following Wiz finding description. Explain the underlying misconfiguration, its potential impact, and provide detailed remediation steps suitable for an engineer new to cloud security:\n\n```
<FINDING DESCRIPTION>
```"
