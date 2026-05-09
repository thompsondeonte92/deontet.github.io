<!-- GitHub Profile README -->

<div align="center">

<svg width="100%" viewBox="0 0 680 180" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Deonte Thompson GitHub Profile Banner</title>
  <desc>PMP Certified Project Professional and evolving cloud architect</desc>
  <rect width="680" height="180" fill="#0a0e1a"/>
  <line x1="0" y1="60" x2="680" y2="60" stroke="#60a5fa" stroke-opacity="0.06" stroke-width="0.5"/>
  <line x1="0" y1="120" x2="680" y2="120" stroke="#60a5fa" stroke-opacity="0.06" stroke-width="0.5"/>
  <line x1="170" y1="0" x2="170" y2="180" stroke="#60a5fa" stroke-opacity="0.06" stroke-width="0.5"/>
  <line x1="340" y1="0" x2="340" y2="180" stroke="#60a5fa" stroke-opacity="0.06" stroke-width="0.5"/>
  <line x1="510" y1="0" x2="510" y2="180" stroke="#60a5fa" stroke-opacity="0.06" stroke-width="0.5"/>
  <rect x="0" y="0" width="680" height="3" fill="#60a5fa"/>
  <rect x="0" y="0" width="680" height="1" fill="#bfdbfe" opacity="0.9"/>
  <rect x="40" y="28" width="3" height="124" fill="#60a5fa" opacity="0.8"/>
  <rect x="48" y="48" width="3" height="84" fill="#60a5fa" opacity="0.3"/>
  <polyline points="648,22 664,22 664,40" fill="none" stroke="#60a5fa" stroke-width="1.5" stroke-opacity="0.55" stroke-linecap="round" stroke-linejoin="round"/>
  <polyline points="32,158 16,158 16,140" fill="none" stroke="#60a5fa" stroke-width="1.5" stroke-opacity="0.55" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="560" y1="20" x2="650" y2="20" stroke="#60a5fa" stroke-opacity="0.12" stroke-width="0.75"/>
  <line x1="580" y1="32" x2="650" y2="32" stroke="#60a5fa" stroke-opacity="0.08" stroke-width="0.5"/>
  <line x1="600" y1="44" x2="650" y2="44" stroke="#60a5fa" stroke-opacity="0.05" stroke-width="0.5"/>
  <text x="62" y="86" font-family="Courier New, monospace" font-weight="700" font-size="42" fill="#e8f4ff" letter-spacing="0.5">Deonte Thompson</text>
  <rect x="62" y="97" width="440" height="1.5" fill="#60a5fa"/>
  <rect x="62" y="98.5" width="440" height="0.5" fill="#bfdbfe" opacity="0.5"/>
  <text x="64" y="118" font-family="Courier New, monospace" font-size="13" fill="#93c5fd" letter-spacing="1.2">Project Professional  ·  Cloud Architecture &amp; Technical Delivery</text>
  <rect x="64" y="133" width="36" height="19" rx="3" fill="#60a5fa" fill-opacity="0.12" stroke="#60a5fa" stroke-opacity="0.7" stroke-width="0.75"/>
  <text x="82" y="146" font-family="Courier New, monospace" font-size="10" fill="#93c5fd" text-anchor="middle">PMP</text>
  <rect x="106" y="133" width="42" height="19" rx="3" fill="#60a5fa" fill-opacity="0.12" stroke="#60a5fa" stroke-opacity="0.7" stroke-width="0.75"/>
  <text x="127" y="146" font-family="Courier New, monospace" font-size="10" fill="#93c5fd" text-anchor="middle">PSM I</text>
  <rect x="154" y="133" width="36" height="19" rx="3" fill="#60a5fa" fill-opacity="0.12" stroke="#60a5fa" stroke-opacity="0.7" stroke-width="0.75"/>
  <text x="172" y="146" font-family="Courier New, monospace" font-size="10" fill="#93c5fd" text-anchor="middle">CCP</text>
  <rect x="196" y="133" width="42" height="19" rx="3" fill="#60a5fa" fill-opacity="0.08" stroke="#60a5fa" stroke-opacity="0.4" stroke-width="0.75"/>
  <text x="217" y="146" font-family="Courier New, monospace" font-size="10" fill="#60a5fa" fill-opacity="0.7" text-anchor="middle">AWS</text>
  <text x="638" y="146" font-family="Courier New, monospace" font-size="10" fill="#60a5fa" fill-opacity="0.5" text-anchor="end">Houston, TX</text>
  <rect x="0" y="176" width="680" height="4" fill="#60a5fa" opacity="0.3"/>
</svg>

</div>

---

## Project Professional. Cloud Architecture & Technical Delivery.

I'm a PMP-certified program and project professional growing deeper into cloud infrastructure, technical delivery, and solutions architecture. I'm building real fluency through hands-on AWS implementation, not just theory or certifications, but actual deployed systems that solve real operational problems.

My background is in administration, leadership, and project management. I know how to run operations, lead teams, manage stakeholders across organizational layers, and bring structure to environments that are still finding their footing. Over time, I found myself paying closer attention to the infrastructure and systems behind the work I was involved in: the way things were architected, where the bottlenecks actually lived, and what it would take to build something better. **That curiosity turned into purpose.**

What makes this interesting is the combination of skill, passion, and natural alignment. I bring operational leadership and delivery discipline into technical conversations, and I bring systems thinking and cloud fluency into delivery work. That intersection is where I do my best work, and it's where I'm continuing to grow.

---

## What I'm Currently Building

### ⬡ AWS Serverless Intake Automation Platform

I built this platform with a specific goal in mind. High volume document processing is one of those problems that looks manageable until it isn't, and I wanted to understand what solving it at the infrastructure level actually requires. The result is a fully serverless, event-driven system on AWS Free Tier that automates document ingestion, OCR extraction, and downstream routing.

**Architecture Overview**

 ![AWS Serverless Intake Automation Platform](https://deontet1.github.io/AWS_Serverless_Intake_Diagram.jpg)


**AWS Services Used**

| Service | Role |
|---|---|
| **S3** | Document ingestion and secure storage |
| **Lambda** | Event-driven processing logic |
| **Textract** | OCR and intelligent document extraction |
| **SNS** | Asynchronous notification and routing |
| **DynamoDB** | NoSQL storage for extracted document data |
| **CloudWatch** | Structured monitoring, alerting, and observability |
| **IAM** | Least-privilege access control across all services |
| **KMS** | Encryption at rest for sensitive document content |

**What This Demonstrates**

- Fully serverless, event-driven architecture with no persistent compute
- Async processing workflows that decouple ingestion from downstream logic
- HIPAA-aligned design considerations including encryption and least-privilege IAM
- Structured CloudWatch monitoring for operational visibility
- End-to-end AWS service integration built from the ground up

> I handpicked this project to force a shift in how I think. From managing work around systems to actually designing them. Building it meant confronting real architectural decisions vs just learning about them.

---

## Skills & Focus Areas

**AWS Services**
`S3` `Lambda` `Textract` `SNS` `DynamoDB` `CloudWatch` `IAM` `KMS`

**Architecture & Technical Concepts**
`Serverless Architecture` `Event-Driven Design` `Asynchronous Processing` `Cloud-Native Thinking` `Systems Thinking` `Observability` `HIPAA-Aligned Design` `Least Privilege Security`

**Professional & Delivery Expertise**
`PMP Certified` `Program Management` `Technical Delivery` `Stakeholder Communication` `Risk Management` `Operational Process Design`

**Growing Into**
`Cloud TPM` `Solutions Architecture` `Implementation Consulting` `Technical Program Management` `Cloud Modernization`

---

## Where I'm Heading

My focus is on roles where delivery leadership and technical depth work together, not separately. That's where I'm investing my time and that's where this work is pointing.

My near-term focus is expanding my AWS depth, exploring infrastructure-as-code, and building out more hands-on architecture projects. Each one teaches me something the classroom doesn't.

---

## Let's Connect

I'm always open to a good conversation, whether you're a recruiter exploring fit, a cloud professional who wants to swap notes, a technical leader with advice to share, or someone curious about the trajectory I'm building.

If something here caught your attention, I'd welcome a conversation, please feel free to reach out.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Deonte%20Thompson-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/deontet/)
[![Project](https://img.shields.io/badge/AWS%20Project-Serverless%20Intake%20Platform-232F3E?style=flat-square&logo=amazonaws&logoColor=white)](#)

---

<div align="center">
<sub>Built with curiosity, deployed with intention. Always learning.</sub>
</div>
