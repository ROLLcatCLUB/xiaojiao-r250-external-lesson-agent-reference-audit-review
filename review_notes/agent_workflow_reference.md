# Agent Workflow Reference

## Reference

saniales/ai-lesson-planner is the cleanest reference for workflow separation. Its useful pattern is that course planning, lesson highlights, detailed discourse, slides, and export are separate roles and artifacts.

## Proposed Xiaobei Workflow Vocabulary

| Proposed role | Responsibility | Output | Boundary |
| --- | --- | --- | --- |
| `unit_planner` | Build 大单元/课程主线, lesson sequence, progression | Unit outline and lesson index | No lesson body writing |
| `source_understander` | Read uploaded/current material and extract source-grounded facts | Source ledger, low-confidence fields, missing info | No invented content |
| `lesson_designer` | Build or repair `single_lesson_template` | Structured lesson template | No formal apply |
| `execution_map_builder` | Turn design into teacher steps, timing, checks | Teacher execution map and classroom timeline | No big-screen binding yet |
| `artifact_maker` | Project accepted template into worksheet, slides, rubric | Candidate artifacts | No R95 export until review |
| `review_agent` | Validate source, teacher readability, completeness, risk | Review report and teacher-confirmation queue | Cannot silently accept model edits |

## Design Principle

The right abstraction is not "more agents". The right abstraction is "one stage owns one artifact boundary". Each role must have a fixed input, fixed output, and explicit non-goals.

## License Boundary

saniales is GPL-3.0 in the local manifest. Do not copy code, agent files, scripts, templates, or directory layout verbatim into Xiaobei. It is acceptable to independently use the architectural idea of staged course-to-lesson-to-slide workflow separation.

## Near-Term Use

Use this workflow reference only after R201/R220 remains stable. For now it can inform naming and future task boundaries, not implementation.

