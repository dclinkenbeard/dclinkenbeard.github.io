---
layout: page
title: CST 338 Redesign
description: Rethinking a 300-level software design course (Java, OOP, design patterns, JavaFX) for the era of generative AI. Working paper, evolving syllabus, and the assessment scaffolding that has to come with both.
img: assets/images/project_cst338/banner.jpg
importance: 1
category: research
---

# CST 338 Redesign: Software Design in the Era of Generative AI

> **TL;DR.** I am redesigning CSUMB's CST 338 (Software Design) from the ground up. The redesign is grounded in a meta-analysis-style literature scan of CS education research, OOP pedagogy, generative-AI-in-CS-education work, and Bloom-for-CS taxonomies. The argument: GenAI does not eliminate the need for programming instruction; it relocates the cognitive bottleneck from syntax to specification, code reading, testing, and design critique. A 300-level course is where students are old enough to do that relocated work.

## Why This Project Exists

CST 338 is a required 300-level course in CSUMB's Computer Science major. Its current Course Learning Outcomes were authored before ChatGPT, before Copilot, and before the field's center of gravity shifted from "should students use AI?" to "what does it mean to teach software design when AI can pass CS1 exams?" The redesign exists to answer the second question for one specific course at one specific teaching-focused institution.

The work has three parts that progress together:

1. **A foundations working paper** that grounds the redesign in peer-reviewed evidence rather than instinct.
2. **A revised CLO architecture** mapped to that evidence and to ABET CAC student outcomes.
3. **The course materials themselves** (assignments, labs, exams, rubrics) rebuilt to align with the revised outcomes.

## Current Status

| Component | Version | Where |
|---|---|---|
| Foundations working paper | v0.1 (May 2026) | [github.com/dclinkenbeard/cst338-redesign-foundations](https://github.com/dclinkenbeard/cst338-redesign-foundations) |
| CLO architecture proposal | Draft (in working paper, Section 5) | same |
| Course materials | In revision for Fall 2026 | private (CSUMB instance) |
| Public blog post | Published May 2026 | [What Should a 300-Level Software Design Course Look Like Now?]({{ site.baseurl }}/blog/2026/cst338-redesign-foundations/) |

## What the Working Paper Argues

In one sentence:

> Generative AI does not eliminate the need for programming instruction; it relocates the cognitive bottleneck from syntax production to specification, code reading, debugging, and design critique. A 300-level software design course is precisely where students are old enough and have enough prior code experience to do the relocated work, and young enough that the habits formed here will define their professional practice.

The paper is structured as the outline of a meta-analysis: working hypothesis, search method, findings across four themes (CS foundations, OOP pedagogy, generative AI in CS education, outcomes and assessment), synthesis of tensions and convergences, implications for CST 338, limitations, and full bibliography.

The bibliography lists twenty peer-reviewed and consensus sources. Eleven are openly available; nine are paywalled and cited by DOI. Verified BibTeX entries are in `sources.bib` in the repo.

## What I Want From Collaborators

Three specific asks (also listed in the working paper itself):

1. **Where is the literature scan thin?** Equity and identity in CS classrooms (Margolis, Fisher, et al.) is the obvious gap and is committed for v0.2. What else?
2. **Where does the proposed CLO architecture break?** I argue for retiring the existing Android CLO. Is that the right call? Am I asking too much of CLO4 (responsible LLM use)?
3. **Where is the GenAI evidence base shakier than the draft makes it sound?** This is the part of the literature I trust least; it is moving fast and most of the strong claims sit on weaker-than-ideal sample sizes.

GitHub issues on the repo are the preferred channel. Email <dclinkenbeard@csumb.edu> works too.

## Roadmap

- **v0.1 (shipped May 2026):** First public draft. Foundations paper, CLO proposal, blog post, this project page.
- **v0.2 (target Fall 2026):** Add the 2025 ITiCSE working-group report *The Rest of the Robots*. Add the equity-and-identity literature. Incorporate colleague feedback from v0.1.
- **v1.0 (target Spring 2027):** Post-deployment revision after one full semester of teaching the redesigned course. Add empirical observations from the deployed assessment scaffolding (Bloom-mapped rubrics, AI-collaboration logs, design-critique grading).
- **Beyond:** Reframe as a submission-ready paper for ITiCSE or SIGCSE if the v1.0 evidence is strong enough.

## How to Cite

If the working paper informs your own teaching or scholarship, cite the tagged release rather than `main`:

> Clinkenbeard, D. A. (2026). *CST 338 Redesign: Foundations for Teaching Software Design in the Era of Generative AI* (Working Paper v0.1). California State University, Monterey Bay. [https://github.com/dclinkenbeard/cst338-redesign-foundations/releases/tag/v0.1](https://github.com/dclinkenbeard/cst338-redesign-foundations/releases/tag/v0.1)

## Acknowledgments

The literature scan, source verification, and document drafting were done with substantial assistance from large-language-model tools (Claude). Every citation was verified against publisher records before inclusion. The working hypothesis, proposed CLO architecture, and pedagogical commitments are my own argument, informed by the cited literature. The same acknowledgment appears in the repo README and the launch blog post.

## License

The foundations working paper and its bibliography are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). Course materials remain CSUMB-instance-internal until and unless they are migrated to a separate public repository.
