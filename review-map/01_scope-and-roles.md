# 01 — Does EU law reach this PRD, and in what role?

Always first. Answer each question with the PRD's own facts; where the PRD is silent, write the question under **decide**.

## AI Act
1. **Is there an AI system?** Definition: [AI Act Art 3(1)](../ai-act/ch-01_general-provisions/art-003.md). A PRD built on Claude or another model counts.
2. **Does the AI Act reach it?** [Art 2(1)](../ai-act/ch-01_general-provisions/art-002.md): providers placing systems on the EU market wherever they are based; deployers in the EU; providers and deployers outside the EU when the system's output is used in the EU.
3. **Is it excluded?** Same article: 2(6) research-only systems, 2(8) research and testing before release, 2(10) a person using AI for purely personal, non-work purposes, 2(12) open-source (with limits). The Commission's reading of the exclusions: [Guidelines §2.5](../guidelines-art5/02_overview-and-scope/2-5.md).
4. **Which role?** Provider (builds it, or has it built, and releases it under its own name) or deployer (uses it at work): [Art 3(3), 3(4)](../ai-act/ch-01_general-provisions/art-003.md), guideline reading at [§2.4](../guidelines-art5/02_overview-and-scope/2-4.md). A deployer or reseller becomes the provider of a high-risk system if it rebrands it, changes it substantially or changes its purpose: [Art 25(1)](../ai-act/ch-03_high-risk-ai-systems/art-025.md). A PRD that wires a model into a tool for other people usually makes its builder a provider.

## GDPR
5. **Is personal information handled?** [GDPR Art 4(1), 4(2)](../gdpr/ch-01_general-provisions/art-004.md). Names, recordings, transcripts, emails and photos all count.
6. **Does the GDPR reach it?** [Art 3](../gdpr/ch-01_general-provisions/art-003.md): an EU establishment, or, from outside the EU, offering goods or services to people in the EU or monitoring their behaviour there. Read with [Recitals 22](../gdpr/recitals/rec-022.md), [23](../gdpr/recitals/rec-023.md), [24](../gdpr/recitals/rec-024.md). Non-EU controllers caught this way need an EU representative: [Art 27](../gdpr/ch-04_controller-and-processor/art-027.md).
7. **Is it excluded?** Purely personal or household activity: [Art 2(2)(c)](../gdpr/ch-01_general-provisions/art-002.md), [Recital 18](../gdpr/recitals/rec-018.md). The tools a household user relies on are still covered: the same recital.
8. **Which role?** Controller (decides why and how) or processor (acts for a controller): [Art 4(7), 4(8)](../gdpr/ch-01_general-provisions/art-004.md). Deciding together makes joint controllers: [Art 26](../gdpr/ch-04_controller-and-processor/art-026.md).

## Result
One line per law: applies / doesn't apply / decide, with the role and the article that decides it. Outside the EU with no EU users, the laws that do apply (national privacy law, for one) are not in this library: see [not-covered.md](not-covered.md).
