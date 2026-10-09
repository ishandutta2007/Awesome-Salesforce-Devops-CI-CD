# Awesome-Salesforce-Devops-CI-CD

## Top Salesforce DevOps & CI/CD Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Metadata Deployment, Release Management & Self-Hosted CI/CD Pipelines*  

**Last updated: October 2026**



This repository tracks notable **commercial Salesforce DevOps platforms** and **open-source projects** that automate metadata deployment, version control, testing, and release management for Salesforce orgs — from click-based release centers to scriptable CI/CD pipelines built on the Salesforce CLI.



**Examples** include Salesforce DevOps Center, Copado, Gearset, AutoRABIT, Flosum, Prodly, Blue Canvas, Salto, Hutte, and Clayton (the category leaders).



**Open-source emphasis**: Salesforce DevOps is a growing open-source domain. **sfdx-hardis** leads as the most complete open-source toolbox with CI/CD pipeline definition, daily metadata backup, org monitoring, and AI-enhanced documentation . **CumulusCI** from Salesforce.org provides battle-tested release automation with org building, dataset loading, and Robot Framework testing . **D2X** delivers composable Salesforce DevOps on GitHub with a container image bundling CumulusCI and Salesforce CLI . **SFDX-Git-Delta** (a core dependency) enables delta deployments by detecting changed metadata between commits . **MegaLinter** integration provides code quality and security scanning . This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Salesforce DevOps Center](https://help.salesforce.com/)**  

  **Salesforce's native, click-based release management** — now generally available as Next-Generation DevOps Center (Spring '26) . **Work items, visual pipelines, and automatic source control** without Git CLI knowledge . **Agentforce Assistant** for natural language merge conflict resolution and deployment fixes . **Support for Bitbucket, data deployment, and combining work items** . **Best for admins and teams wanting native Salesforce DevOps** .



- **[Copado](https://www.copado.com/)**  

  **The leader in AI-powered DevOps for Salesforce**, 100% native to Salesforce . **Agentia™** embeds context-aware AI agents across Plan, Build, Test, Release, and Operate stages with built-in governance, audit trails, and role-based access controls . **Agentia Context Hub** grounds agents in org metadata, dependencies, pipelines, and history . **6 specialized DevOps agents + Orchestrate Agent** for multi-step workflow management . **Best for enterprises wanting governed AI-powered DevOps** .



- **[Gearset](https://gearset.com/)**  

  **The most trusted Salesforce DevOps platform** — compare and deploy, Git integration, CI/CD, unit testing, and data deployment . **Native Gitflow support in Pipelines** — bundle features into release branches, move through dev → test → staging → production . **PR Queuing** sequences merges automatically to eliminate race conditions . **Continuous Delivery Rules** auto-promote changes when trusted conditions (validations passed, tests succeeded, code reviewed) are met . **Layered Modules** for global core + regional flexibility . **Chrome Extension** brings admins into the same workflow as developers . **Best for enterprise teams at scale** .



- **[AutoRABIT](https://www.autorabit.com/)**  

  **Enterprise DevSecOps platform for Salesforce** — CI/CD, code quality, backup/recovery, and security posture . **ARM** (Automated Release Management) for deployments and rollbacks . **CodeScan** for static code analysis and policy management . **Vault** for automated backup, recovery, and sandbox seeding . **Guard** for security and compliance monitoring . **Parallel Processor** fires POST requests before/after deployments for notifications and integrations . **Best for regulated industries needing DevSecOps** .



- **[Flosum](https://www.flosum.com/)**  

  **Purpose-built Salesforce DevSecOps platform** — DevOps, backup/archive, and security orchestration in one . **Agentic DevOps** for managing Agentforce deployments with safe agent deployment, goal-driven release management, and governance at machine speed . **Cloud and self-hosted deployment** for data residency compliance . **Trusted by Fortune 100 companies including Cargill** . **Best for enterprises scaling Agentforce** .



- **[Prodly](https://prodly.co/)**  

  **Salesforce data deployment and DevOps** — CPQ, Vlocity, and advanced data migrations.



- **[Blue Canvas](https://bluecanvas.io/)**  

  **Salesforce version control and backup** — Git-based metadata versioning with automated backups.



- **[Salto](https://www.salto.io/)**  

  **SaaS configuration management** — deploy and manage Salesforce and other SaaS configurations.



- **[Hutte](https://hutte.io/)**  

  **Salesforce DevOps platform** — scratch org management and CI/CD.



- **[Clayton](https://clayton.io/)**  

  **Salesforce code quality and security** — static analysis and governance.



## Open-Source GitHub Projects



### CI/CD Toolboxes & Pipelines



- **[sfdx-hardis](https://github.com/hardisgroupcom/sfdx-hardis)**  

  **The most complete open-source Salesforce DevOps toolbox**, presented at Dreamforce 23 and 24 by Cloudity . **Orchestrates base Salesforce CLI commands** with interactive wizards for complex operations . **Defines complete CI/CD Pipeline** for Salesforce projects — ready to use with most platforms and tools . **Daily Metadata backup and org monitoring** for any Salesforce org . **AI-enhanced project documentation** including AI-generated descriptions and Flow Visual History . **Docker images for CI** with Node.js, Salesforce CLI, sfdx-hardis, and plugins pre-installed . **Standard images** (without coding agent CLIs) and **with-agents images** (Claude, Codex, Gemini, GitHub Copilot pre-installed for AI-powered auto-fix scenarios) . **Best for comprehensive open-source Salesforce DevOps**.



- **[CumulusCI](https://github.com/SFDO-Tooling/CumulusCI)**  

  **Salesforce.org's complete development and release process**, open-source (not covered by Salesforce Master Subscription Agreement) . **Builds sophisticated orgs with automatic dependency installation** . **Loads and captures sample datasets** to make orgs feel real . **Applies transformations to existing metadata** for org-specific requirements . **Runs builds in CI systems** with end-to-end browser testing via Robot Framework . **Generates synthetic data at any scale** via Snowfakery (from one record to a million) . **Portable automation** stored in source repository — runs from local CLI, CI system, or MetaDeploy installer . **Works with scratch orgs and persistent orgs** (sandboxes, production, Developer Edition) . **Best for ISV and complex org release automation** .



- **[D2X](https://pypi.org/project/d2x/)**  

  **Composable Salesforce DevOps on GitHub**, created by MuseLab . **Defines a container image for Salesforce development, build, and delivery** using CumulusCI and Salesforce CLI . **Consistent runtime environment** for automation across the entire software product lifecycle . **Aligns with Salesforce's Well-Architected Framework** . **Used as the framework for all of MuseLab's services engagements** and shared freely with the ecosystem . **Best for teams wanting containerized Salesforce CI/CD**.



### Deployment & Delta Tools



- **[SFDX-Git-Delta (sfdx-git-delta)](https://github.com/scolladon/sfdx-git-delta)**  

  **Generates delta packages from Git commits**, open-source . **Core dependency for sfdx-hardis and many Salesforce CI/CD pipelines** . **Only deploys changed metadata** between commits, dramatically reducing deployment time and risk . **Essential for large orgs where full deployments are impractical** . **Best for delta deployments in CI/CD** .



- **[SFDX-Falcon](https://github.com/buttjc/sfdx-falcon)** — Salesforce DX template for advanced package development .



- **[sfpowerkit](https://github.com/Accenture/sfpowerkit)** — Accenture's Salesforce DX plugin with org operations, metadata management, and CI/CD helpers .



### Testing & Quality



- **[MegaLinter](https://github.com/oxsecurity/megalinter)**  

  **Open-source code quality and security linter aggregator**, used by sfdx-hardis Docker images . **Salesforce-specific flavor** available (megalinter-salesforce) . **Runs multiple linters in one pass** including Apex, LWC, and metadata checks . **Best for CI-based Salesforce code quality** .



- **[Apex PMD](https://github.com/pmd/pmd)** — Static analysis for Apex with Salesforce-specific rules .



- **[ESLint Aura](https://github.com/forcedotcom/eslint-plugin-aura)** — Linting for Aura components .



- **[Prettier Apex](https://github.com/dangmai/prettier-plugin-apex)** — Code formatting for Apex .



### Additional Strong Open-Source Options



- **Salesforce CLI** — Official CLI for Salesforce DX, foundation for all open-source tooling .

- **SFDX-Git-Delta** — Delta package generation for efficient deployments .

- **SFDX-Data-Move-Utility (SFDmu)** — Data migration and sandbox seeding tool .

- **Snowfakery** — Synthetic data generation for Salesforce testing at scale .

- **Robot Framework** — End-to-end testing framework integrated with CumulusCI .

- **ApexTestKit** — Apex test data factory library .

- **SFDX-Profiles** — Profile and permission set management tool .

- **Texei-SFDX-Plugin** — Texeï's Salesforce DX plugin with org and metadata helpers .



**Frameworks for building custom Salesforce DevOps solutions**: Combine **sfdx-hardis** for comprehensive CI/CD pipelines, daily backups, and org monitoring with Docker-based execution . Use **CumulusCI** for ISV-grade release automation with org building, dataset loading, and Robot Framework testing . Deploy **D2X** for containerized, composable DevOps on GitHub . Integrate **SFDX-Git-Delta** for delta deployments that only push changed metadata . Use **MegaLinter** for code quality and security scanning in CI . Note that true enterprise Salesforce DevOps with AI-powered release management, governance at machine speed, and vendor-supported SLAs (Copado Agentia, Gearset, AutoRABIT) remains primarily commercial territory; open-source stacks provide strong CI/CD pipelines, delta deployments, and org monitoring foundations that require integration for complete Salesforce DevOps.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Salesforce DevOps platforms handle sensitive org metadata, configuration, and potentially production data. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **CumulusCI is distributed under an open-source license and is not covered by the Salesforce Master Subscription Agreement** . Review the license before commercial use.

- **Delta deployments are critical for large orgs** — SFDX-Git-Delta is the foundation for efficient CI/CD. Full deployments become impractical as metadata volume grows .

- **License considerations**: sfdx-hardis is open-source , CumulusCI is open-source , D2X is open-source , and SFDX-Git-Delta is open-source . Verify licensing against your use case before committing.

- The open-source ecosystem provides strong CI/CD pipelines, delta deployments, and org monitoring foundations, but **AI-powered release management, governance at machine speed, and vendor-supported SLAs** remain primarily commercial offerings.



---



**Made for Salesforce developers, admins, release managers, and organizations seeking Salesforce DevOps sovereignty.**  

Let's make Salesforce DevOps and CI/CD more open, transparent, and automated.
