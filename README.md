# Deonte Thompson — Program Manager turned Cloud Architect 🏗️

📍 Houston, TX &nbsp;|&nbsp; AWS SAA Candidate &nbsp;|&nbsp; PMP · PSM · CCP

---

## About

For six years I managed the programs that ran on enterprise infrastructure — SaaS implementations, cross-functional delivery workstreams, regulated environments where data accuracy and access controls weren't optional. I learned what breaks, what costs money, and what slows teams down.

That experience is what drives the work here. I'm not building proof-of-concepts in a vacuum — I'm designing the systems I watched organizations need, using the architecture patterns that actually hold up under compliance scrutiny and operational load. The shift from managing delivery to engineering the solution is deliberate, and it's informed by everything that came before it.

Currently pursuing **AWS Solutions Architect Associate**. BS in Cloud & Network Engineering at WGU (expected Jan 2027).

---

## 🔧 What I'm Building

### AWS Serverless Intake Automation Platform

Organizations processing high volumes of intake documents face a persistent bottleneck: manual data entry is slow, error-prone, and unscalable. I've seen it firsthand — in biotech, in healthcare, in any environment where intake volume is high and the margin for error is low. This platform replaces that manual workflow with a fully serverless, event-driven pipeline on AWS.

```
┌─────────────┐   S3 Event    ┌──────────────┐   Start Job   ┌─────────────────┐
│  Document   │──────────────▶│   Lambda      │──────────────▶│  Amazon         │
│  Upload (S3)│               │  (Trigger)    │               │  Textract       │
└─────────────┘               └──────────────┘               └────────┬────────┘
                                                                       │
                                                              Async Completion
                                                                       │
                                                                       ▼
┌─────────────┐  Store Record ┌──────────────┐  SNS Notify   ┌─────────────────┐
│  DynamoDB   │◀──────────────│   Lambda      │◀──────────────│  Amazon SNS     │
│  (Output)   │               │  (Processor)  │               │  (Notification) │
└─────────────┘               └──────────────┘               └─────────────────┘
       │                              │
       └──────────────────────────────┘
                        │
                        ▼
        ┌───────────────────────────┐
        │      Amazon CloudWatch    │
        │   Logs · Metrics · Alarms │
        └───────────────────────────┘
```

**Design decisions that mattered:**
- **Async processing via SNS** — decouples Textract job completion from Lambda execution, eliminating timeout risk on large or complex documents
- **Least-privilege IAM** — each Lambda has a dedicated execution role scoped to only what it needs. No wildcard policies on production resources
- **KMS encryption** — SSE-KMS on S3 and DynamoDB at rest; HTTPS enforced in transit. HIPAA-aligned by design, not by retrofit
- **Structured CloudWatch logging** — unstructured `print()` statements don't scale across concurrent invocations. Audit trail built in from day one

**Projected impact:** 70% reduction in manual document processing · 60% faster intake cycle time

**Services:** `S3` `Lambda` `Amazon Textract` `SNS` `DynamoDB` `CloudWatch` `KMS` `IAM`

---

## 🏅 Credentials

![PMP](https://img.shields.io/badge/PMP-Certified-0052CC?style=flat)
![PSM](https://img.shields.io/badge/PSM%20I-Certified-009FDA?style=flat)
![CCP](https://img.shields.io/badge/AWS%20CCP-Certified-%23FF9900?style=flat&logo=amazon-aws&logoColor=white)
![SAA](https://img.shields.io/badge/AWS%20SAA-In%20Progress-%23FF9900?style=flat&logo=amazon-aws&logoColor=white)
![WGU](https://img.shields.io/badge/BS%20Cloud%20%26%20Network%20Engineering-WGU%202027-003087?style=flat)

---

## 🛠️ Tech Stack

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=flat&logo=amazon-aws&logoColor=white)
![Lambda](https://img.shields.io/badge/AWS%20Lambda-%23FF9900?style=flat&logo=aws-lambda&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-%234053D6?style=flat&logo=amazondynamodb&logoColor=white)
![S3](https://img.shields.io/badge/Amazon%20S3-%23569A31?style=flat&logo=amazons3&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SNS](https://img.shields.io/badge/Amazon%20SNS-%23FF9900?style=flat&logo=amazon-aws&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-%23FF4F8B?style=flat&logo=amazon-aws&logoColor=white)
![IAM](https://img.shields.io/badge/IAM-Least--Privilege-%23DD344C?style=flat&logo=amazon-aws&logoColor=white)
![KMS](https://img.shields.io/badge/KMS-Encryption-%23FF9900?style=flat&logo=amazon-aws&logoColor=white)

---

## 📊 GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=thompsondeonte92&show_icons=true&theme=github_dark&hide_border=true)

---

## 📬 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-deontet-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/deontet)
[![Email](https://img.shields.io/badge/Email-1deonte.thompson%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:1deonte.thompson@gmail.com)
