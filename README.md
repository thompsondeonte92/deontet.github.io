<p align="center">
  <img src="./deonte_thompson_banner_final.svg" alt="Deonte Thompson Banner" width="100%"/>
</p>

<br/>

```
Certified Project Manager · Cloud Enthusiast
Houston, TX  |  PMP · PSM I · AWS CCP
BS Cloud & Network Engineering (In-progress)
```

---

## `> whoami`

PMP, PSM I, and AWS CCP certified Program Manager with experience across biotech, startups, nonprofits, education, and consumer sectors. I bring structure to moving parts and help teams stay aligned — especially when things get complex.

What drives me is **clarity**. Taking something complicated and making it understandable: a delivery timeline, a cross-functional dependency, a system architecture. That same instinct is what pulled me toward cloud. I started seeing the infrastructure behind the programs I was managing and got curious about building it myself. That curiosity turned into hands-on work.

My goal is to move fully into **Cloud Program Manager** and **Technical Program Manager** roles — environments where the work is meaningful, teams are collaborative, and cloud is at the center of how things get built. That's where I'm headed.

Currently completing my **BS in Cloud and Network Engineering** at WGU.

---

## `> ls projects/`

### ⚡ AWS Serverless Intake Automation Platform

Organizations processing high volumes of intake documents face a persistent bottleneck: manual data entry is slow, error-prone, and unscalable. This platform replaces that manual workflow with a fully serverless, event-driven pipeline on AWS.

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
- **KMS encryption** — SSE-KMS on S3 and DynamoDB at rest, HTTPS enforced in transit. HIPAA-aligned by design, not by retrofit
- **Structured CloudWatch logging** — unstructured print statements don't scale across concurrent invocations. The audit trail is built in from day one

**Projected impact:** `70%` reduction in manual document processing · `60%` faster intake cycle time

`S3` `Lambda` `Textract` `SNS` `DynamoDB` `CloudWatch` `KMS` `IAM`

---

## `> cat credentials.txt`

![PMP](https://img.shields.io/badge/PMP-Certified-0052CC?style=flat)
![PSM](https://img.shields.io/badge/PSM%20I-Certified-009FDA?style=flat)
![CCP](https://img.shields.io/badge/AWS%20CCP-Certified-%23FF9900?style=flat&logo=amazon-aws&logoColor=white)
![WGU](https://img.shields.io/badge/BS%20Cloud%20%26%20Network%20Engineering-WGU%202027-003087?style=flat)

---

## `> cat stack.txt`

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

## `> cat stats.txt`

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=thompsondeonte92&show_icons=true&theme=github_dark&hide_border=true"/>
</p>

---

## `> contact --open`

[![LinkedIn](https://img.shields.io/badge/LinkedIn-deontet-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/deontet)

---

<p align="right">
  <sub><code>// Houston, TX · building in the open</code></sub>
</p>
