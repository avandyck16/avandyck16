## 👾 Welcome to Axel's GitHub 👾

---

### Who's behind all of this? 

- A QA Engineer with strong foundations and hands-on experience in manual and automated testing.

- Here is a collection of professional, academic, and personal projects fully documented, each with its own repository and detailed case study, including metrics, technical challenges, implemented solutions, code snippets, and visual evidence of the final results.

---

### ➡️ Current Stack

<p align="center">
      <img src="https://skills.syvixor.com/api/icons?perline=8&i=azure,cypress,playwright,k6,jest,visualstudiocode,javascript,selenium,yaml,powershell,postman,markdown,chatgpt,windows,apple,android" />
  </p>


<!--
<p align="center">
      <img src="https://skillicons.dev/icons?i=azure,cypress,javascript,vscode,selenium,powershell,postman,md,ai,windows,apple" />
  </p>
-->

### ➡️ Latest / Current Professional Experience

>**Alset, Inc. | QA Engineer | Test Automation & Manual E2E Testing**


---

>_As a professional teacher in my past years, I learned from and worked with former National Geographic Education and Pearson’s top consultant, seeing many students conquer challenges across areas and life stages. This taught me the value of continuous learning and purposeful work, which I now apply in my day by day._

---


<div align="center">
  <a href="https://drive.google.com/file/d/1ZvK-cUYmKfiLjfps08EoIOuZR-Hhqjcq/view?usp=drive_link" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/Ver_CV-PDF-red?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="View Resume">

</a>
  <a href="https://drive.google.com/file/d/1Z9jP0Dpa02uQiOxV9WXs-7lCnD1wPOhU/view?usp=drive_link" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/View_Resume-PDF-red?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="View Resume">
</a>

<a href="https://github.com/avandyck16?tab=repositories">
   <img src="https://img.shields.io/badge/View_Repositories-%23121011.svg?style=for-the-badge&logo=github&logoColor=white">
</a>

<!-- <a href="https://qa-warrior.notion.site/Projects-Portfolio-08a7f2a1544a48d391cd91eaa5423c2d">
   <img src="https://img.shields.io/badge/View_Case_Studies_at_Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white">
</a>
--> 

 
</div>

<br>

<div align="center">
   
[![acontreras9012@gmail.com](https://skillicons.dev/icons?i=gmail)](mailto:acontreras9012@gmail.com) [![LinkedIn](https://skillicons.dev/icons?i=linkedin)](https://linkedin.com/in/axelvandyck)   
   
</div> 

---

# 💼 Featured Projects

## 3PLICITY 
#### E2E Automation Framework; B2B Logistics SaaS | Cypress | JavaScript | Azure Pipelines | CI/CD

- E2E automation for a SaaS logistics management platform focused on operations between 3PL companies and merchants.
- Reduction of manual validation time from ~1.15 hours to ~2.42 minutes **(~96%)**.
- The implementation of this framework enabled the automation of critical processes within a SaaS logistics platform, covering complete workflows between different user roles and business operations.
- The solution reduced dependency on manual validations, improved regression reliability, and enabled earlier detection of issues throughout the delivery lifecycle.

    ➡️ [View Case Study](https://github.com/avandyck16/3PLicity-Supply-Chain-Platform-E2E-Automation)

---

## SprintLine
#### E2E Automation Framework | Cypress | JavaScript | Azure Pipelines | CI/CD

- E2E automation for an AI-powered platform that transforms product ideas into technical documentation and implementation-ready specifications.
- Validation time reduced from ~50 minutes to ~9 minutes **(~82%).**
- The framework automates critical workflows including authentication, registration, Questionnaire, Product Definition, and RFP generation and delivery.
- Its Azure DevOps integration enables tests to run against the build artifact before deployment, preserve execution evidence, and incorporate E2E validation into the CI/CD process.
- Result: a stable and repeatable E2E automation suite providing representative coverage of SprintLine's highest-value workflows and direct integration with the software delivery pipeline.

    ➡️ [View Case Study](https://github.com/avandyck16/Sprintline-Automated-Testing-JS-Cypress)

---

## Brandhub
#### E2E Automation Framework | Cypress | JavaScript | Azure Pipelines | CI/CD

- E2E automation suite using Cypress for BrandHub, an AI-powered branding platform with generative AI integrations.
- Reduced validation time from ~45 min to ~5 min **(88%).**
- Beyond reducing manual validation effort before deployment, the solution addressed technical challenges involving backend cold starts, unstable selectors, asynchronous rendering, persistent sessions, dynamic test data, generative AI response times, and automated reporting.
- The implementation of this E2E automation suite enabled automated validation of critical BrandHub workflows while integrating testing directly into the CI/CD process.

    ➡️ [View Case Study](https://github.com/avandyck16/BrandHub-Testing-Cypress-JS-Azure)

---

## Pipeline CI/CD v1.1.1 — Environment-Aware Build & E2E Quality Gate
#### Vite + Cypress + Azure DevOps + Azure Static Web Apps

- Refactor of an existing CI/CD pipeline to align application builds, Cypress E2E validation, environment configuration, and deployment targets according to the branch being processed.
- Although pipeline architecture was not my primary role, I went beyond implementing the Cypress test stages and investigated how the CI/CD workflow operated as a whole.
- As the automation framework evolved, this approach introduced a limitation: **Production deployments were being validated using a Development build and Development configuration**.
- The pipeline was therefore redesigned so that the build, Cypress configuration, and deployment target are aligned with the branch being processed.

- #### Branch-Based Deployment

| Merge target | Build | Cypress            | Deploy |
| ------------ | ----- | ------------------ | ------ |
| `dev`        | DEV   | DEV configuration  | DEV    |
| `main`       | PROD  | PROD configuration | PROD   |

  ➡️ [View Case Study](https://github.com/avandyck16/Pipeline-CICD-Environment-Aware-E2E-Gate)

---

## Automation Implementation | Pipeline CI/CD 
#### Vite + Cypress + Azure Static Web Apps 

>Beyond test automation: I am not a Pipeline or DevOps Architect, but I wanted to go beyond simply writing tests. I took the initiative to understand how CI/CD pipelines work, how the different stages interact, and how QA automation could become part of that process. >This project was the result of putting that knowledge into practice and building the initial testing pipeline for the team.

- This automation framework was initially integrated into the CI/CD workflow through Azure DevOps YAML pipelines, incorporating Cypress E2E test execution as a quality gate before deployment.
- This YAML file defines an automated workflow that builds the application on a controlled dev environment, runs end-to-end Cypress tests, and deploys to Azure Static Web Apps depending on the branch (`dev` or `main`).
- The goal is that every time someone performs a push or merge, the system handles the complete process without manual intervention.
- The logic implemented was:

| Situation      | Initial Build | Cypress | Build PROD | Deploy |
| -------------- | ------------- | ------- | ---------- | ------ |
| PR → `dev`     | DEV           | DEV     | —          | —      |
| Merge → `dev`  | DEV           | DEV     | —          | DEV    |
| PR → `main`    | DEV           | DEV     | —          | —      |
| Merge → `main` | DEV           | DEV     | PROD       | PROD   |

   ➡️ [View Case Study](https://github.com/avandyck16/Pipeline-CI-CD-Vite-Cypress-Azure)

---

## IT Management Tools | Historical Project
#### Administrative Tools Collection | Batch | CMD | PowerShell 

- IT MGMT TOOLS is a collection of administrative utilities for Windows developed in Batch (.bat), designed to centralize common system maintenance, diagnostics, recovery, and configuration tasks into a single menu-based interface.
- The main goal was to reduce the time required to perform repetitive technical support tasks, avoiding the need to manually remember or type multiple commands during maintenance and troubleshooting processes.
- This project was developed around 2011–2012, several years before my professional transition into QA Engineering and Automation.
- Although the project was created more than a decade ago, several of its features remain useful today, and some are still part of my workflow for diagnostics and maintenance tasks in Windows environments.


    ➡️ [View Case Study](https://github.com/avandyck16/it-management-tools-axel)

---

## 😄 Facts About Me  

→ I started breaking and fixing computers when I was 12. Thanks, dad, for bringing our first old PC home back then — you accidentally started my QA journey! 

→ Intuitive ability is my main weapon.

→ I taught myself 3D modeling for a video game by experimenting with software and game assets at age 16.  

→ I created a Windows maintenance toolkit over a decade ago to automate support tasks—and I still use parts of it today.
(You can take a look at it in my repositories)

→ I’m still growing, but I’ve reached the point where I know I can bring real value to the team

→ I enjoy diving into new software tools and getting up to speed with them quickly.

---

<div align="center">
   
[<img width="773" height="447" alt="githublogos" src="https://github.com/user-attachments/assets/728f594e-f45a-43b6-b12b-7d4bc541b2d4" />](https://linkedin.com/in/axelvandyck)

</div>
   
---
<div style="text-align:center; color:#888; font-size:10px;">
    Axel Van Dyck | QA Engineer | 2026
</div>

   
