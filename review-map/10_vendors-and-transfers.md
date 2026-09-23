# 10 — Outside tools, vendors, and data leaving the EU

For PRDs that use an AI API, SaaS, cloud storage, connectors (Zoom, Notion, SharePoint, image generators) or any other party.

## Who is who
1. Each outside tool that handles personal data for the PRD is usually a processor. The controller needs a contract with the terms in [GDPR Art 28(3)](../gdpr/ch-04_controller-and-processor/art-028.md), and may only use processors that give enough guarantees: 28(1). Why: [Recital 81](../gdpr/recitals/rec-081.md). Processors act only on instructions: [Art 29](../gdpr/ch-04_controller-and-processor/art-029.md).
2. If a vendor decides its own purposes with the data (training its models on it, for one), it may be a controller or joint controller: [Art 26](../gdpr/ch-04_controller-and-processor/art-026.md). Mark **decide** unless the PRD names the vendor's terms.
3. The controller stays responsible overall: [Art 24](../gdpr/ch-04_controller-and-processor/art-024.md).

## AI value chain
4. Suppliers of tools, models or components to a high-risk system must agree in writing what information and access the provider needs: [AI Act Art 25(4)](../ai-act/ch-03_high-risk-ai-systems/art-025.md) (rewritten 2026). A model maker must give those building on its model the information in [Art 53(1)(b)](../ai-act/ch-05_general-purpose-ai-models/art-053.md), [Annex XII](../ai-act/annexes/annex-12.md).

## Transfers outside the EU
5. Personal data may leave the EU only under [Chapter V](../gdpr/ch-05_international-transfers/CONTEXT.md): an adequacy decision ([Art 45](../gdpr/ch-05_international-transfers/art-045.md)), safeguards such as standard contract clauses ([Art 46](../gdpr/ch-05_international-transfers/art-046.md)), binding corporate rules ([Art 47](../gdpr/ch-05_international-transfers/art-047.md)), or a narrow exception ([Art 49](../gdpr/ch-05_international-transfers/art-049.md)). General rule: [Art 44](../gdpr/ch-05_international-transfers/art-044.md). Where does each tool store and process the data?

## Watch
- Which countries currently hold an adequacy decision isn't in this library: [not-covered.md](not-covered.md).
