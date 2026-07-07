# Xiaobei Adoption Plan

## Current Priority

Do not interrupt the current chain:

```text
R201/R220 first
R201M model patch as candidate only
R220F center-body readonly route canary
```

R250 is planning evidence, not a new implementation branch.

## Phased Adoption

| Phase | Timing | What to borrow | Output |
| --- | --- | --- | --- |
| Phase 0 | Now | Reference audit only | R250 docs |
| Phase 1 | After R201/R220 route is stable | Free-prep input schema and source-understanding boundary | R240 intake contract |
| Phase 2 | After R240 has stable entry | Agent/workflow split | Unit-to-lesson workflow spec |
| Phase 3 | After R230 surface contract | Classroom timeline and big-screen page mapping | `teacher_execution_map` and `classroom_timeline` contract |
| Phase 4 | After teacher review gate is mature | Multi-artifact bundle shape | R95 export readiness |
| Phase 5 | After R210 safety policy | Xiaojiao in-class support suggestions | Readonly/support mode first |

## Acceptance Criteria Before Any Runtime Reuse

Any external-project-inspired capability must pass:

- Capability classification: design-only, template-only, deterministic transform, model call, local write, network call, dependency/runtime.
- License review.
- Dependency review.
- Data and privacy review.
- Source ledger compatibility.
- Teacher review gate compatibility.
- Rollback path.
- Preview-only smoke before formal apply.

## Recommendation

The immediate next useful artifact after R250 is not code. It is a Xiaobei-native `teacher_execution_map` contract that bridges `single_lesson_template` to classroom timeline and big-screen page planning while staying readonly.

