# review-map — check one PRD against the laws

One job: read one PRD, decide which EU rules reach it, and report what it breaks, misses or leaves open. Hand-written; the law files it links to are generated.

## Inputs
- Working (this run): the PRD file the user names — normally a chalky-prd output (sections: Mission, 1 Problem, 2 Constraints, 3 Outputs, 4 Inputs, 5 Steps, 6 Artifact breakdown, 7 Open questions).
- Reference (every run): this file, [01_scope-and-roles.md](01_scope-and-roles.md), [timeline.md](timeline.md), [not-covered.md](not-covered.md).
- Reference (as picked below): the area files the table sends you to, then only the article files those point at.

## Process
1. Read the PRD once, whole. List its facts: who builds it, who uses it, which countries, whose information goes in, what the AI does, what comes out and who sees it, decisions made about people, outside tools and vendors.
2. Work through [01](01_scope-and-roles.md). If no EU law reaches the PRD, say so, give the reason in one line, list what would change that, and stop. If it depends on a fact the PRD doesn't give, carry on as if the law applies and say what it depends on under Scope.
3. Pick areas from the table. Always add [02](02_prohibited-practices.md) as a quick screen.
4. For each area, answer its questions from the article files it links, never from memory. Files flagged `changed_2026` or marked `▼M1` differ from the 2024 text.
5. For anything you flag, check [timeline.md](timeline.md): a rule that isn't in force yet is still a finding, marked with its date.
6. Write the report (below).

| The PRD says or implies… | Read |
|---|---|
| the AI talks to people, or makes images, audio, video or text others will see | [04](04_transparency-and-ai-literacy.md) |
| sexual images, or fakes of real people | [02](02_prohibited-practices.md), [04](04_transparency-and-ai-literacy.md) |
| nudging, persuasion, targeting children, disabled or poor people | [02](02_prohibited-practices.md) |
| face, voice, emotion or body-based recognition | [02](02_prohibited-practices.md), [03](03_high-risk.md), [04](04_transparency-and-ai-literacy.md) |
| decisions, scores or rankings about people: jobs, school, credit, insurance, benefits, access to services | [03](03_high-risk.md), [08](08_automated-decisions.md) |
| information about identifiable people: names, emails, recordings, transcripts, photos | [06](06_personal-data-basics.md), [07](07_transparency-and-rights.md), [09](09_security-and-design.md), [11](11_records-and-assessments.md) |
| health, disability, biometrics, ethnicity, religion, sexuality, politics, union, crime | [06](06_personal-data-basics.md), [12](12_special-contexts.md) |
| children, school, staff or workplace use, research | [12](12_special-contexts.md) |
| outside AI, APIs, SaaS, cloud, connectors; data stored or sent outside the EU | [10](10_vendors-and-transfers.md) |
| trains, fine-tunes or offers a model to others | [05](05_general-purpose-ai-models.md) |
| staff will use AI tools, or the PRD writes AI rules for an organisation | [04](04_transparency-and-ai-literacy.md) (AI literacy) |
| anything flagged above, to size the risk | [13](13_penalties.md) |

## Outputs
A report, written where the user says — never into this library or into chalky-prd:
- **Scope** — which laws apply and why, in 2–3 lines, naming the role (provider, deployer, controller, processor).
- **Findings** — one per issue: PRD section · what it says · the rule (cite as `AI Act Art 26(1)`, `GDPR Art 6(1)(f)`, `GDPR Recital 71`, `Art 5 Guidelines para 243`) · the words of the rule that matter, quoted · what to change. Mark each **breaks**, **missing**, or **decide** (depends on a fact the PRD doesn't give).
- **Not checked** — anything relevant from [not-covered.md](not-covered.md), one line each.

## Human check
For every finding marked **breaks** or **missing**, open the cited article and confirm the quoted words are there and say what the finding claims.
