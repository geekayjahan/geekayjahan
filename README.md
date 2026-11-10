# Hi, I'm GK

I'm Gayathri Keerthana (GK), an ex-Amazon Senior Product Manager. I build AI agent products for my own two businesses and for clients, and I teach the method I build with. The method is spec engineering: writing down what you want built so precisely that AI agents can build it correctly, with evals that prove the build works.

This profile holds the things I have built that way, how I keep them safe, and the free kits from my lessons.

## Things I've built

| Project | What it does | Proof |
|---|---|---|
| [followthrough](https://github.com/geekayjahan/followthrough) | My entry to the Meta Global AI Developer Hackathon. A WhatsApp back office for owner-run businesses that tracks every open deal and drafts the next move for approval. [3-minute demo](https://youtu.be/WgxoR8faiuA) | 97 automated checks run on every push. An approval is tied to the exact draft, so an edited draft cancels the earlier yes. [Controls and known limits](https://github.com/geekayjahan/followthrough/blob/main/SECURITY.md) |
| [mise](https://github.com/geekayjahan/mise) | The workspace I run both businesses from. One grid of every lead and customer, where each fact shows its source and age, and background jobs keep mail, leads and the books current. Source is private. [3-minute demo](https://github.com/geekayjahan/mise/blob/main/demo/mise-demo.mp4), or [my own walkthrough on Loom](https://www.loom.com/share/e3558290ddee467c9e2ee1bb72354acf) | A fact past its shelf life shows as unknown. Nothing is sent or posted without my approval. |
| SEO audit tool for an agency client | A prospect's URL goes in and a shareable six-pillar audit comes back in under five minutes, for use on live sales calls. In production since November 2026. Source is private because it is client work. | 80 written acceptance checks. Three graded eval runs took failed checks from 4 to 0. Any AI finding the crawl cannot support is dropped before it is stored, and each report runs under a £1 cost ceiling. |
| [gks-exec-assistant](https://github.com/geekayjahan/gks-exec-assistant) | A project manager plugin for Claude, with portable templates for other platforms | |
| [omnisavant](https://github.com/geekayjahan/omnisavant) | A dashboard that classifies how AI companies build lasting advantages | |

## How I keep them safe

An agent that reads messages and writes to real systems needs controls you can point to in the code. These are the rules I build to. followthrough is the public example, and each row names what is in its code today.

| Rule | How it shows up in followthrough |
|---|---|
| Nothing leaves without a person's yes | The agent drafts and the owner approves. The approval is bound to a hash of the exact draft. |
| Outside content is data, never instructions | WhatsApp and email text reaches the model labelled as untrusted, and the answer must fit a fixed shape before the app acts on it. |
| Keys never touch the repo | Secrets live only in the host's variables, and two secret scans run on every push. |
| History is checked as well as the current files | A privacy test reads every commit, because a file can be clean while an older commit still publishes the data. |
| Dependencies are watched | Dependabot proposes updates weekly, CI fails on a high-severity advisory, and every GitHub Action is pinned to a commit. |
| Limits are written down | [SECURITY.md](https://github.com/geekayjahan/followthrough/blob/main/SECURITY.md) lists what is not yet covered, next to what is. |

## Learn with me on Maven

| Offer | What you get | When |
|---|---|---|
| [**Product Builder Certification by GK**](https://maven.com/level-up-with-ai/product-builder-certification-spec-driven-ai-agents?utm_source=github&utm_medium=profile&utm_campaign=pbc-dec26&utm_content=gh-profile) | A two-week live course. You write a spec for a real problem, direct a team of AI agents in Claude Code to build from it, prove it works with evals, and deploy it. No coding background needed. | 4 to 19 Dec 2026 |
| [**One-day workshop: From Vibe Coding to Spec Engineering**](https://maven.com/level-up-with-ai/product-builder-certification-spec-engineering-beyond-vibe-coding?utm_source=github&utm_medium=profile&utm_campaign=ws-dec26&utm_content=gh-profile) | One fast pass of the method in 5.5 live hours, for people who want the core before committing to the course. | 13 Dec 2026 |
| [**Raise Your Technical Bar as an AI-Native PM** (free recording)](https://maven.com/level-up-with-ai/o/8dd031?utm_source=github&utm_medium=profile&utm_campaign=rytb-recording&utm_content=gh-profile) | The lesson I co-hosted with Jason P. Yoong: 15,700 signups, featured by Lenny Rachitsky. It covers system instructions and evals, which the course turns into a full build. | On demand |
| [**Training for product teams**](https://maven.com/level-up-with-ai/o/05233d?utm_source=github&utm_medium=profile&utm_campaign=teams&utm_content=gh-profile) | A private version for your team. Maven can invoice your company directly. | On request |

## Free lesson kits

Each repo is the working material from a live lesson, so you can rebuild the demo on your own problem.

| Repo | Lesson | What you can do with it |
|---|---|---|
| [ll6-gk-hamza-spec-lesson](https://github.com/geekayjahan/ll6-gk-hamza-spec-lesson) | Spec Engineering for FDEs, with Hamza Farooq | Turn kickoff notes into a `spec.json` and run a check that catches a build ignoring the client's data rules |
| [boundaries-for-agents](https://github.com/geekayjahan/boundaries-for-agents) | Vibe-coding the Agent Owner Spec, with Jason P. Yoong | Fill a ten-field spec that sets what an agent may do, when it stops and how it recovers |
| [ai-chief-of-staff-lesson](https://github.com/geekayjahan/ai-chief-of-staff-lesson) | Build Your Own AI Chief of Staff | Two prompts and a Claude project that brief you every weekday morning |
| [ai-chief-of-staff](https://github.com/geekayjahan/ai-chief-of-staff) | Template version | Six prompts for Claude Code that end with your own installed plugin |
| [skills](https://github.com/geekayjahan/skills) | AI Bar Raiser post on agent files | A skill that builds and audits other Claude skills |

## Experience

- **Founder and Director, Flywheel by GK and Kāma Coffee** (Bristol, 2025 to now). I teach spec engineering on Maven, where I am a Top 100 Product & AI instructor rated 4.7 out of 5, and I ran an AI-adoption workshop for 100+ PMs at Canva. I also build agentic systems for small businesses; one saves a client's leadership team 15 hours a week across 210 accounts. Kāma Coffee is my speciality coffee brand, which I run solo across e-commerce and wholesale to UK cafés.
- **Senior Product Manager, Amazon** (UK, 2021 to 2024). I worked with applied scientists to turn a Bayesian ML model into a product and launched ML-driven 24-hour delivery across the EU and UK, part of a £250M delivery-speed programme in a £5.6B business unit.
- **Pathways Operations Manager, Amazon.** I ran operations at a robotics fulfilment centre with 5 managers and 300 associates, producing 200K units a shift at 98.7% delivery accuracy.
- **B2B SaaS growth, Zoho and Chargebee** (2015 to 2019). I led inbound and demand generation at Chargebee and ran demand generation, partner marketing and attribution at Zoho. During my MBA I interned on product growth at Typeform.
- **Founder, Connect for a Cause** (2013 to 2019), a non-profit protecting women and children in rural India. It ran awareness programmes for 22,000+ children and won the state-level Seva Ratna Award.
- International MBA, Esade. BE in Computer Science, Avinashilingam University. UK Global Talent Visa for Exceptional Talent in Digital Technology.

Full history on [LinkedIn](https://www.linkedin.com/in/gayathri-keerthana/).

## Writing

I write [**AI Bar Raiser**](https://aibarraiser.substack.com?utm_source=github&utm_medium=profile&utm_campaign=substack&utm_content=gh-profile) on Substack, about building with AI from first principles and the operating mechanisms frontier labs use.

## Get in touch

[Book a call](https://calendly.com/flywheelbygk-info/1-on-1-gk) or email info@flywheelbygk.com.
