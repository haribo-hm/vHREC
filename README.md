# vHREC

**Virtual Human Research Ethics Committee.** AI decision support for human research ethics review, research governance and study monitoring. People decide; vHREC drafts.

![The vHREC workbench after a review of an invented study](docs/screens/overview.jpg)

> **Status.** A working product, tested end to end on synthetic research projects. It has not yet been validated on genuine submissions, and we have no customers or revenue yet. We are looking for pilot partners: human research ethics committees, research governance offices and trial sponsors.

## Demo

A five-minute walkthrough on an invented study will be posted here shortly.

## What it does

One upload of a research submission package (protocol, participant information and consent forms, ethics application, data management plan and the rest) becomes six things.

1. **A pre-screen against Australia's National Statement on Ethical Conduct in Human Research (2025).** Each finding names where in the submission it arises, quotes the researcher's text where it can, and cites the passage of the National Statement it rests on. It is written for the researcher: what to change, where, why, and what to send back.
2. **A human checkpoint.** The ethics officer keeps, discusses or excludes each finding. Nothing reaches a researcher until a person has decided.
3. **A simulated committee sitting.** A multi-seat AI panel, with a seat for each membership category the National Statement requires, reviews the project. It debates the contested points under a chair, votes, and drafts the outcome letter. A deliberation map shows who changed position and why.
4. **Governance paperwork.** The site-specific assessment checklists are filled only where a verbatim quote from the submission supports the entry. The memos, authorisation letter and data custodian request are generated from them as Word documents.
5. **A draft research monitoring plan.** The plan gives the study's NHMRC (2018) risk category, the monitoring intensity that category starts from, the risks that raise it, and the checks each risk calls for. Each risk is tied to the Clinical Trials Transformation Initiative's critical-to-quality factors. The plan downloads as Word for a monitoring professional and the sponsor to complete.
6. **Learning at the point of need.** Short lessons on what review bodies look for are offered beside the findings that raise them. There are paths for first-time applicants, researchers, coordinators, committee members, ethics officers and monitors.

| Findings, as the researcher reads them | The committee's deliberation map |
|---|---|
| ![Findings written for the researcher](docs/screens/findings.jpg) | ![Who moved, on which issue](docs/screens/committee.jpg) |
| **Governance: a field filled from a verified quote** | **A draft research monitoring plan** |
| ![Governance checklist with a verified quote](docs/screens/governance.jpg) | ![Monitoring plan with risks and checks](docs/screens/monitoring-plan.jpg) |

![The monitor's learning path](docs/screens/learn.jpg)

## How it is built

- **Rules first.** A deterministic engine raises findings with their evidence. Models add judgement where rules cannot, and a model's quote is checked against the source text before it is shown.
- **Hosted or on-premises.** It runs on a hosted model (the demo uses Thinking Machines' Inkling through OpenRouter) or on open-weight models on the institution's own hardware. A real-submission lock refuses hosted model endpoints.
- **Drafts, not decisions.** Every output is a draft for the human committee or office. vHREC makes no ethics or governance decision.
- **Tested.** About 2,900 automated tests.

## Who it is for

- Human research ethics committees, and the research governance offices behind them.
- Trial sponsors and contract research organisations preparing submissions and monitoring studies.
- Institutions that want the workbench under their own name, with models tuned on their own records and run on their own infrastructure.

## The company

CDTR X vHREC is a contract research organisation in Queensland, Australia, focused on digital therapeutics. It uses custom AI products to support ethics and governance review and clinical trial delivery. It offers three things:

- **CRO services:** trial management, ethics and governance submissions, and monitoring.
- **Consulting.**
- **AI-enabled software:** the vHREC workbench, available white-label.

## Team

- **Hari K Muralidharan**, co-founder: research ethics and governance.
- **Maame Amma Owusu**, co-founder: clinical trials auditing and monitoring.

## Contact

<!-- Add the contact address before the page is made public. -->
Contact details to follow.

---

This repository is the project page only. The vHREC software is not published here. The screenshots show an invented study at an invented institution, the fictional Wattle Coast Hospital and Health Service. On the committee map, public figures stand in as review lenses for the committee's seats.
