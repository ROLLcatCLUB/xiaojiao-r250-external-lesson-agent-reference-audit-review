# Free Prep Input Schema Reference

## Reference

DivanshiJain2005/AI-lesson-planner is a minimum viable lesson-plan form demo. It is not a deep architecture reference, but its field list is useful for the lowest-friction free-prep entry.

## Minimum Fields

| Field | Required | Why |
| --- | --- | --- |
| `lesson_title` | yes | Identifies the lesson topic |
| `subject` | yes | Drives discipline-specific language |
| `grade` | yes | Calibrates developmental level |
| `duration_minutes` | yes | Enables pacing and timeline feasibility |
| `key_vocabulary` | optional | Helps focus core concepts |
| `supporting_materials` | optional | Gives teacher-provided sources |

## Xiaobei Extensions

Xiaobei should add these fields before treating the input as a serious source-grounded prep request:

| Field | Required for source-grounded generation | Reason |
| --- | --- | --- |
| `textbook_version` | recommended | Aligns to教材/版本 |
| `unit_title` | recommended | Places lesson in unit progression |
| `curriculum_standard_or_stage` | recommended | Avoids generic objectives |
| `teacher_intent` | recommended | Captures what the teacher actually wants changed |
| `material_condition` | recommended | Distinguishes uploaded source, pasted outline, no material |
| `generation_mode` | yes | Chooses baseline-only, candidate patch, free draft, or review-only |

## Risk Notes

The Divanshi app has a hardcoded placeholder API key line, uses an old `openai==0.28.0` requirement, and directly calls a provider from the Streamlit app. This is not compatible with Xiaobei's provider gate, source policy, or teacher review gate.

## Adoption Rule

Borrow only the input-field simplicity. Do not borrow provider handling, UI implementation, dependency versions, or generation strategy.

