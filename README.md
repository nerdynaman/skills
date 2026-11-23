<p align="center"><img src="assets/hero.svg" alt="Skills — reusable instructions for focused agent work" width="100%"></p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-SKILL.md-7C3AED" alt="Markdown skill format">
  <img src="https://img.shields.io/badge/Skills-3-334155" alt="Three focused skills">
</p>

Three focused agent skills: **understand technical articles**, **write grounded job-application messages** and **create concise visual READMEs**. Each is a readable Markdown playbook in its own folder.

## Pick a skill

| Skill | What it does |
| --- | --- |
| [Understand technical articles](Understand-technical-articles/SKILL.md) | Explains a technical article through eight questions, then helps you explore a chosen topic more deeply. |
| [Job application message](job-application-message/SKILL.md) | Writes an 80–120-word hiring-team message connecting a specific role to relevant, verified experience. |
| [Polish README](polish-readme/SKILL.md) | Builds a concise, factual repository front page with useful visuals; handles descriptions and publishing when requested. |

```mermaid
flowchart LR
    A[Article or job description] --> B[Choose a skill]
    B --> C[Read its SKILL.md]
    C --> D[Your agent follows the playbook]
```

## Use

```sh
git clone https://github.com/nerdynaman/skills.git
cd skills
```

Point your agent at the skill’s `SKILL.md`, or copy its folder into the skill directory your agent supports. Example prompts:

> Read `Understand-technical-articles/SKILL.md` and use it to explain this article: [link].

> Read `job-application-message/SKILL.md` and draft a message for this job description: [text].

> Read `polish-readme/SKILL.md` and improve this repo’s README with useful visuals. Keep the repository visibility unchanged.

**Personalize before reuse:** the job-message skill contains the author’s background. Replace it with your own verified experience before drafting applications.

## What to expect

- Article explanations cover the problem, main idea, mechanism, prerequisites, choices, trade-offs, evidence and applications.
- Application messages use role-specific details and avoid invented experience or generic company praise.
- README updates preserve setup and recovery details, verify links and visuals, and keep publication within the requested scope.
- These are instructions for your agent, not a standalone application. Link access depends on the tools your agent has available.
