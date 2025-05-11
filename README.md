# 📘 DevOps Prompt Collection for Effective AI Assistance

A collection of carefully crafted prompts DevOps engineers can use with AI tools like ChatGPT to get accurate and actionable results. Suitable for day-to-day troubleshooting, automation, documentation, and optimization tasks.

---

## 1. 🧪 Analyze CI/CD Pipeline Errors

```text
Analyze this CI/CD pipeline error and suggest possible fixes:

[Paste your error logs here]

Context:
- We're using GitHub Actions with a Node.js application
- Tests pass locally but fail in the pipeline
- This started happening after upgrading dependencies yesterday
```

---

## 2. 📑 Convert Infrastructure Description into Documentation

```text
Convert this infrastructure description into clear, comprehensive documentation with appropriate sections:

[Describe your infrastructure components, connections, and dependencies]

Please include:
1. A high-level architectural overview
2. Key components and their purposes
3. Data flow between services
4. Security considerations
5. Common failure points and mitigations
```

---

## 3. 💾 Create MySQL Backup Script

```text
Create a bash script that:
- Backs up all MySQL databases
- Compresses the backups
- Uploads them to S3
- Deletes backups older than 7 days
- Sends a status email with success/failure details

Include error handling, logging, and comments explaining complex parts. I'm running this on Ubuntu 22.04
```

---

## 4. 📊 Optimize Prometheus Alerting Rules

```text
Help me optimize these Prometheus alerting rules:

[Paste your current alerting rules]

We're experiencing:
- Too many false positives for CPU spikes
- Missing alerts for actual database connection issues
- Alerts that don't provide enough context for triage

Our environment: Kubernetes cluster with 30 microservices, primarily Go and Java applications, PostgreSQL and Redis for storage.
```

---

## 5. ☁️ Generate Terraform Code for AWS Infra

```text
Generate Terraform code for AWS infrastructure with:
- Load-balanced web tier in 2 availability zones
- Auto-scaling application tier
- RDS database with read replicas
- S3 for static assets with CloudFront CDN
- Appropriate security groups and IAM roles
- Tags for all resources for cost allocation

Include documentation comments and follow Terraform best practices for organization and variable usage.
```

---

## 6. 🐳 Troubleshoot Kubernetes Deployment Issues

```text
Troubleshoot this Kubernetes issue:

Symptoms:
- Pods continuously crash and restart
- Error logs show: [paste relevant logs]
- Started after deployment of version 1.4.2 yesterday

Environment:
- GKE Kubernetes 1.26
- Istio service mesh 1.14
- Application uses 1.2GB memory according to resource requests

What I've tried:
- Restarting the deployments
- Checking for CPU/memory pressure
- Reviewing recent configuration changes
```

---

## 7. 🚨 Create MySQL Incident Response Runbook

```text
Create a comprehensive incident response runbook for our MySQL database failures.

Include:
- Initial assessment steps
- Common causes and their specific symptoms
- Step-by-step recovery procedures for each scenario
- Escalation criteria and contact information
- Post-incident analysis template

Make it accessible for engineers with basic database knowledge but who aren't database experts.
```

---

## 8. 🛡️ Analyze Vulnerability Impact

```text
Analyze this vulnerability (CVE-2023-XXXXX) for our environment:

Vulnerability details:
[Paste details from security advisory]

Our environment:
- 40 microservices running Java 17 and Node.js 18
- Using Spring Boot 2.7.x and Express 4.x
- Containerized with Docker, deployed on Kubernetes
- External-facing APIs behind Cloudflare WAF

Provide:
1. Assessment of our potential exposure
2. Specific services/components likely affected
3. Immediate mitigation steps
4. Long-term remediation plan
```

---

## 9. 💸 AWS Cost Optimization Based on Tags

```text
Analyze these AWS cost allocation tags and suggest optimization strategies:

Monthly costs by service:
[Paste your cost breakdown]

Usage patterns:
- Dev environments run 24/7
- Nightly batch processing between 1-4 AM
- Traffic peaks between 9 AM - 6 PM weekdays
- Multiple RDS instances at standard tier
- Several underutilized EC2 instances

Provide:
1. Immediate cost-cutting opportunities
2. Medium-term architectural changes for efficiency
3. Automation suggestions for resource scheduling
4. Recommendations for right-sizing resources
```

---

## 10. 📝 Write a Blameless Postmortem

```text
Help me write a blameless postmortem for this incident:

Incident details:
- 4-hour service disruption on our payment processing system
- Root cause: Database connection pool exhaustion
- Contributing factors: Unexpected traffic spike, insufficient monitoring
- Resolution: Increased pool size, added circuit breakers

Write a comprehensive postmortem that:
1. Focuses on systems and processes, not individuals
2. Clearly explains the timeline and impact
3. Analyzes contributing factors
4. Proposes specific, actionable improvements
5. Highlights what went well in the response
```

---

✅ **Tip:** When pasting logs, configurations, or descriptions, provide as much context as possible for more precise responses.
