# riverpod.rfc
Submissions repository for `ASOC3` - Self-Hostable Podcasting Platform

> [!NOTE]
All discussions regarding `ASOC3: Self-Hostable Podcasting Platform` shall take place in https://github.com/orgs/acm-avv/discussions/11.

## Overview
In-order to be eligible to work on this project as **Request for Code** under the banner of **Amrita Summer of Code, 2025**, you are required to form a team of size 1-4 and have all the members register at [amsoc.vercel.app](https://amsoc.vercel.app)

## Project Manager Details
@vijay-sb
```json
"Name": "Vijay S B, Vasudev Kishor",
"Year": "3rd",
"Roll": "CB.SC.U4CSE23249, CB.SC.U4CSE23151",
"GitHub": "@vijay-sb, @VasudevKishor",
```

## How to Apply
Type out a message in https://github.com/orgs/acm-avv/discussions/11 with the following details:
1. Team Name
2. Team Members' Names, Roll-Numbers and respective GitHub usernames
3. Tag the project manager as **@username**

## Guidelines
1. Keep all discussions limited to this discussion channel by tagging the project manager via **@username**
2. Do not try to contact the project manager personally unless they are open to it.
4. Maintain decorum and avoid any misbehavior with the project manager. This can be subjected to disqualification.
5. Send us an update every week with regards to your progress for your respective project. If we do not receive an update for more than 10 days then your team will be disqualified automatically.

---
## Project Description

A **Self-Hostable Podcasting Platform** will be developed, offering functionalities similar to Riverside.fm, with a focus on comprehensive audio/video recording, editing, and distribution.

* **Platform Goal:** To provide a self-hostable solution for podcast creation and management, akin to Riverside.fm.

* **Technology Stack:**
    * **Web App (Frontend):**
        * React (not Next.js)
        * TypeScript
        * ShadCN (UI component library)
        * Tanstack Router (or similar routing library)
    * **Backend App:**
        * Express (web application framework)
        * DrizzleORM (Object-Relational Mapper)
        * TypeScript
        * Zod (schema validation library)
        * PostgreSQL (database)

* **Key Integrations & Features:**
    * **Media Processing:** FFMPEG (for multimedia handling), Transcoding Pipelines.
    * **Real-time Communication:** WebRTC (for real-time audio/video), WebSockets (for real-time communication).
    * **Storage:** Minio (or a pluggable S3-compatible file-storage solution).
    * **Content Delivery:** CDNs (Content Delivery Networks).

* **Deployment & Orchestration:**
    * Entire distributed system managed via Podman and Nomad (as an alternative to Docker + Kubernetes).

* **Project Structure:**
    * The entire project will be contained within a single repository using TurboRepo (the monorepo framework).
