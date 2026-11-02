# Supplier Update Triage — 77-second walkthrough

[Open or download the captioned video](walkthrough.mp4)

This silent walkthrough uses actual implementation captures from my [supplier triage capstone](https://github.com/JasonTeixeira/tripleten-ai-automation-portfolio/tree/main/projects/supplier-delay-triage). It is a local prototype with fictional emails, not a customer deployment or a newly recorded live LLM run.

| Time | Inspect |
| --- | --- |
| 0:00 | Complete connected n8n workflow |
| 0:11 | Custom extraction prompt and schema |
| 0:22 | Ollama request mapping and captured AI output |
| 0:33 | Original email paired with the AI response |
| 0:44 | Business rules for exceptions and manual review |
| 0:55 | Persisted SQLite records from a separate captured run |
| 1:06 | Controlled LLM outage routed to manual review |

The original captures are in [`evidence/reviewer-fix`](https://github.com/JasonTeixeira/tripleten-ai-automation-portfolio/tree/main/projects/supplier-delay-triage/evidence/reviewer-fix): files 01, 04, 06, 07, 13, 12, and 17, in that order. Screenshots remain unaltered apart from video scaling; new captions occupy separate margins. The SQLite capture and workflow canvas represent different recorded runs, so their route counts are not combined as one execution.

The local automated checks passed **42 tests on November 2, 2026**. They check validation and workflow contracts; they do not establish live-model accuracy or operational savings. The project documentation includes reproduction instructions and limitations.
