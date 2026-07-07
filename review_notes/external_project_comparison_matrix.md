# External Project Comparison Matrix

## Summary

The four repositories answer different questions:

| Project | Best reference value | Our mapping | Adoption priority | Do not adopt now |
| --- | --- | --- | --- | --- |
| Claw-ED | Complete lesson bundle, quality gate, teacher style, approval/risk classification | Future R95 output package, quality sentinel, teacher review policy | High for design shape | Do not import runtime, provider layer, scheduler, browser, Telegram, Google Drive, or self-modifying tools |
| saniales/ai-lesson-planner | Course-to-lesson-to-slides workflow split, artifact folders, handoff prompts | R240 free prep planning, R200/R201 decomposition, future artifact chain | High for workflow design | Do not copy GPL-3.0 code or agents directly |
| classmin | Classroom timeline, PPT page references, student-state simulation, Xiaojiao-like execution support | R210 Xiaojiao control, R230 big screen/right rail, R250 classroom simulation planning | High for later classroom execution | Do not connect CrewAI/AutoGen/Chroma/Ollama stack to mainline now |
| DivanshiJain2005/AI-lesson-planner | Minimum free-prep input and simple output shape | R240 minimum free-prep intake schema | Low to medium | Do not use code as security or architecture reference |

## Evidence Snapshot

Claw-ED README describes complete lesson bundles with plans, handouts, slides, differentiated versions, games, and teacher voice. It also documents teacher DOCX, student DOCX, slides PPTX, a quality gate with 12 pedagogical checks, local-first trust model, export formats, and a central risk/approval policy.

saniales README and agent files split work into `course-planner`, `discussion-moderator`, `lesson-planner`, `slides-maker`, and PDF export. Its `course-planner` explicitly does course outline and metadata, not lesson-level content.

classmin README describes CrewAI lesson-prep output as `教案`, `PPT脚本`, `说课稿`, and `课堂时间线`; its simulation side models time, PPT page references, activity types, and student understanding/attention/frustration.

Divanshi is a Streamlit/OpenAI demo with fields such as lesson title, subject, grade, duration, key vocabulary, and supporting materials/resources. It has a hardcoded placeholder API key line and old OpenAI package dependency, so it is only useful for minimum input shape.

## Current Xiaobei Chain Implication

These projects confirm a product direction: a lesson-generation system should not stop at a single text draft. However, the immediate chain is still `single_lesson_template + source policy + teacher review gate + readonly center-body route`. R250 should feed planning, not implementation.

