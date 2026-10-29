# Trackemy

![Trackemy logo](./assets/logo.png)

> **Trackemy doesn't just manage your school, it preserves your child's entire educational journey, forever.**

**A school management platform for Nepal, built on a permanent student-identity spine.**

[![Status](https://img.shields.io/badge/status-web%20in%20active%20development-yellow)]()
[![Mobile](https://img.shields.io/badge/mobile-in%20development-yellow)]()
[![Market](https://img.shields.io/badge/market-Nepal%20%C2%B7%2030%2C000%2B%20schools-blue)]()
[![License](https://img.shields.io/badge/license-Proprietary-red)]()

---

## The One-Line Story

Trackemy is an all-in-one school management SaaS that connects principals, teachers, students, and parents  **and preserves each student's educational history permanently**, even after they leave the school.

Most school software sells admin features to principals. Trackemy sells **emotion to parents and students** while still delivering the admin value principals need.

Our philosophy is one sentence: **your school records belong to you, forever.**

---

## The Problem

Nepal has **30,000+ schools**, and the overwhelming majority still run on paper:

- Manual attendance registers, no parent visibility, no accountability
- Student records lost when a student transfers, or when the school changes software
- Cash fee collection, no receipts, no audit trail, no digital payment
- No parent–teacher communication channel beyond phone calls and paper notes
- No longitudinal view of a student's growth from Class 1 to Class 10

When a school leaves a software vendor (or closes, or the student transfers), the student's history is **gone**. Existing platforms treat a student as a row inside one school's database, not as a person with a 10-year academic life.

---

## The Solution

Trackemy is built on a **permanent student identity**, a single, never-recycled `student_id` that is the spine of the entire platform. Everything else hangs off it: enrollments, attendance, marks, report cards, health records, transfer history, memories.

This architecture makes three features possible that no Nepali competitor offers, and that no global platform offers cleanly.

---

## 👑 The Three Crown Jewels

These are Trackemy's differentiators, ranked by emotional and marketing power. All three tell one consistent story.

### 1. Lifetime Student Record (Alumni Mode) - Emotion 10/10

> *"Your school memories, preserved forever."*

After Class 10 or after the school leaves Trackemy, the student retains full read-only access to their history, **free forever**.

- Alumni Mode: read-only lifetime access at zero cost
- Viral potential: a graduated student sharing a Class 1 photo or result is free marketing
- Storage cost per student over a lifetime is less than NPR 5, goodwill vastly exceeds cost
- Competitors lock or delete value when a school leaves; **Trackemy preserves it for the student**

### 2. Digital Academic Passport - Emotion 9/10

> *"Your child's history follows them, wherever they go."*

When a student transfers schools, their history travels with them automatically, securely, with parent consent.

- New teachers immediately understand a student's strengths and weaknesses
- No paperwork, no lost report cards, no starting from zero
- Secure transfer token with parent OTP, privacy protected by design
- Long-term: the foundation for a national student ID system for Nepal

### 3. Student Longitudinal Record - Emotion 8.5/10

> *"Watch your child grow, year by year."*

Every mark, attendance entry, and behavioral note from Class 1 to Class 10 in one permanent, portable profile.

- Teachers see a student's entire academic journey before meeting them
- Principals identify school-wide patterns across years
- Parents watch their child grow on a single timeline
- Never lost, even if the school changes software or closes

**Engineering note:** #3 is the technical spine that makes #1 and #2 real. Without the permanent `student_id` architecture from day one, none of the three is achievable.

---

## Platform Features

### Web Platform (in active development)

- Daily attendance with real-time parent push notifications
- Assignment and exam management
- In-app teacher–parent chat (group and 1-on-1)
- Fee management with **eSewa** and **Khalti** digital payments
- PDF marksheet and report card generation
- Role-based access for principals, admins, teachers, parents, and students

### In Development

- **Mobile applications** (Android + iOS) - actively being built
- **School Memory Vault** - school memories anchored to the academic timeline; 1 GB free per student, paid storage above
- Fingerprint / biometric gate integration for arrival and departure notifications
- **Student Academic Profile Sharing**, Class 10+ students 
  can share verified academic profiles directly with colleges 
  and universities for admission consideration

---

## What Exists Today

Trackemy is in **active development** across web and mobile. The full system is being built end-to-end, database, backend, and frontend, with a deliberate focus on getting the architecture right before any real school data lands.

The underlying database schema has been designed and hardened for production ahead of launch. This is unusual at this stage, and reflects how seriously we take the "records belong to you, forever" promise.

What this means in practice:

- The permanent student identity spine is implemented and working
- The transfer passport token system is implemented
- The memory vault quota and storage system is implemented
- The schema is production-hardened: explicit cascade policies on every financial and audit relation, composite indexes on high-volume tables, partial unique constraints enforced at the database level, and a documented set of production invariants that the code is required to honor
- Sensitive edits to attendance and exam results are audit-trailed at the row level, who edited, what the original value was, and why

A more detailed technical overview is available on request under NDA. The codebase is maintained in a private repository.

---

## Early Validation

Trackemy is not a slide deck. It is a product with a real pipeline:


-   **School conversations beginning across Koshi Province**
- **Municipal education officer interest confirmed** by Shivasatakshi Municipality
- **PABSON Jhapa district connection established** with the PABSON district president, who has expressed interest
- Multiple private and community schools in Dharan, Biratnagar, Itahari, and Damak in early discussions

The go-to-market is Koshi-first, and the response in the region has been strong. This is the foundation for the year-one target of 100–150 paying schools.

---

## Market & Strategy

| Horizon | Target |
|---|---|
| Total addressable market | 30,000+ schools across Nepal |
| Year 1 | 100–150 paying schools |
| Year 2 | 500+ schools plus municipal (palika) partnerships |
| Long term | Government MOU with the Ministry of Education, Science and Technology (MoEST) |

### Koshi Province First

Our go-to-market starts where we have home-ground advantage:

- Deep local networks and cultural understanding
- Eastern Nepal is the least penetrated region for the incumbent competitor
- District-level word-of-mouth spreads organically, one happy principal talks to ten others
- Hundreds of untouched community schools are a natural freemium funnel

**Phased expansion:** Koshi (Month 1–8, 50–100 schools) → Province 1 + Madhesh (Month 8–14, 100–300 schools) → all seven provinces (Month 14–20, 500–1,000 schools) → national government engagement (Month 18–24, with scale and data as proof).

### Why This Is Not Playing Small

Every major Nepali company started with home-ground advantage. Nail Koshi first, and let word of mouth reach Kathmandu before we do, that's more powerful than starting in Kathmandu with no roots.

---

## Business Model

- **Schools:** annual SaaS subscription, tiered by student capacity. Freemium available to land community schools and expand from there.
- **Alumni:** free forever, basic lifetime view. Goodwill, loyalty, and organic word-of-mouth,not a revenue line.
- **School Memory Vault (in development):** 1 GB free per student; paid storage above that. A passive add-on, not core revenue.

Detailed pricing is shared with schools directly and with investors as part of the data room.

---

## Why Trackemy Wins

### Against the incumbent (Veda)

We do not compete head-to-head. We compete differently:

- Target the **~28,000 schools** not yet on any platform, the majority of the market
- Position as the **next-generation** platform, not a re-implementation of a 2015-era product
- Veda was not designed around parents; Trackemy was
- Freemium and community-school motion expands the market rather than fighting over existing accounts

### Against global platforms

| Platform | Lifetime / Alumni (free) | Cross-school Transfer Passport | Full Longitudinal Record |
|---|---|---|---|
| **Trackemy** | **Yes** | **Yes** | **Yes** |
| PowerSchool (US) | No | No | District-only |
| Alma (US) | No | No | Partial |
| iSAMS (UK) | No | No | Enterprise-only |
| Classplus (India) | No | No | Coaching-only |

The combination of **Lifetime Alumni Mode (free forever)** + **cross-school Digital Academic Passport** + **Longitudinal spine** is, to our knowledge, not offered by any platform globally, not just in Nepal.

### Brand

The name **Trackemy** (track + academy) is unique, self-explanatory, and owns its keyword entirely,zero competition in SEO. It reads as a funded SaaS product in Nepal and internationally. The primary domain and social handles are secured.

---

## Team

A focused founding team of **two**,  technical depth and commercial depth, no overlap, no filler.

### Yogendra Baskota, Tech Head, Engineering

Electronics, Communication and Information Engineer. Full-stack AWS engineer with three years at multiple Nepali technology companies. Responsible for:

- End-to-end platform architecture and database design
- Backend services, cloud infrastructure, and security posture
- Web and mobile application development
- Production operations and data-protection safeguards

🔗 [LinkedIn](https://www.linkedin.com/in/yogendrabaskota)

### Suman Baskota, Sales Head, Commercial

Lawyer and sales professional. Responsible for:

- School acquisition across Koshi Province and beyond
- Municipal and government relationship-building
- Commercial contracts, data-handling policy, and regulatory compliance
- Investor and grant-partner relations

🔗 [LinkedIn](https://www.linkedin.com/in/suman-baskota)

The company is bootstrapped and registered in Nepal as **Rook Technology Pvt. Ltd.**

---

## Roadmap

| Phase | Focus |
|---|---|
| Current | Web platform in active development; mobile application in development |
| Next 2 quarters | Web and Mobile (Android + iOS) launch; first paying schools in Koshi Province |
| Following year | Multi-province expansion; palika-level partnerships |
| Long term | National-scale student identity infrastructure; government MOU |

---

## For Developers and Technical Partners

The Trackemy codebase is **maintained in a private repository**. It is not open source at this time.

If you are evaluating Trackemy as a technical partner, investor with technical due diligence, or infrastructure provider, a controlled technical walkthrough can be arranged under NDA. Please contact us using the details below.

We are **not accepting external contributions** at this time.

---

## Contact

- **General and investor inquiries:** [info@trackemy.com](mailto:info@trackemy.com)
- **Founder, Engineering:** [yogendra@trackemy.com](mailto:yogendra@trackemy.com)
- **Founder, Commercial:** [suman@trackemy.com](mailto:suman@trackemy.com)
- **Security disclosures:** [security@trackemy.com](mailto:security@trackemy.com)
- **Website:** [trackemy.com](https://trackemy.com)
- **LinkedIn:** [linkedin.com/company/rook-technology](https://www.linkedin.com/company/rook-technology)

---

## Legal

Trackemy is a product of **Rook Technology Pvt. Ltd.**, registered in Nepal.

**Copyright © Rook Technology Pvt. Ltd.** All rights reserved.

This repository and all associated materials are proprietary. No part of this document may be reproduced, distributed, or transmitted in any form without prior written permission from Rook Technology Pvt. Ltd.

Trackemy handles minors' educational data and takes its obligations under Nepal's Privacy Act 2018 seriously. Data-handling, consent, and retention policies are documented and available to prospective schools and partners on request.

---

> *Your school records belong to you, forever.*