# R250 External Lesson Agent Reference Audit

Stage ID: `1013R_R250_EXTERNAL_LESSON_AGENT_REFERENCE_AUDIT`

R250 is a read-only reference audit for four external teacher-prep GitHub projects. It uses them to calibrate what a mature lesson-generation system can become, not to replace or mutate the current Xiaobei/师维智教 chain.

## Decision

These projects are useful as a design reference library. They are not current implementation references for R201, R220, R210, R95, or runtime provider wiring.

Current protected chain remains:

1. `R201 / R220`: stabilize `single_lesson_template` and center-body readonly route.
2. `R201M`: model patch is teacher-review-required candidate only.
3. `R220F`: R97B center-body route canary remains readonly and does not bind right rail, bottom Xiaojiao, export, write, or provider/model calls.

External projects can inform later R240, R230, R210, and R95 planning after the current route and template line is stable.

## Sources

- External repos: `Z:\SmartEdu-External-References\teacher-prep-github-refs-20260708-051212`
- Manifest: `Z:\SmartEdu-External-References\teacher-prep-github-refs-20260708-051212\reference_manifest.json`
- Current R201M package: `outputs/PREP_ROOM_RENDER_CANVAS_DEEPEN_V1/1013R_R201M_MODEL_PATCH_GATE_AND_TEACHER_REVIEW_PREVIEW`
- Current R220F package: `outputs/PREP_ROOM_RENDER_CANVAS_DEEPEN_V1/1013R_R220F_R97B_CENTER_BODY_READONLY_ROUTE_BINDING_CANARY_WITH_PATCH_PREVIEW`

## Files

- `external_project_comparison_matrix.md`: project-to-Xiaobei comparison.
- `lesson_bundle_output_chain_reference.md`: Claw-ED-inspired future output package shape.
- `agent_workflow_reference.md`: saniales-inspired agent/workflow separation.
- `classroom_simulation_and_xiaojiao_reference.md`: classmin-inspired classroom timeline and Xiaojiao execution support.
- `free_prep_input_schema_reference.md`: Divanshi-inspired minimum free-prep input schema.
- `xiaobei_adoption_plan.md`: phased adoption plan that preserves current R201/R220 priority.
- `do_not_adopt_risks.md`: explicit non-adoption and risk list.
- `r250_source_evidence_map.json`: exact source file and line evidence used.
- `r250_boundary_verification.json`: readonly boundary verification.

## Boundary

R250 did not copy code, install dependencies, run external projects, call providers/models, modify backend/frontend runtime, modify R201/R220/R210/R95, write database/Feishu/memory, or create formal exports.

