# Classroom Simulation And Xiaojiao Reference

## Reference

classmin is the strongest reference for classroom execution rather than lesson prose. It combines a CrewAI prep pipeline with a manual classroom simulation loop, time tracking, PPT page references, and rule-based student state.

## Useful Concepts

| classmin concept | Xiaobei/Xiaojiao interpretation |
| --- | --- |
| `课堂时间线.md` parsed into structured stages and steps | Future `classroom_timeline` derived from accepted `single_lesson_template` |
| Teacher `[PPT页]` references | Future link between teacher execution step and big-screen page |
| `[用时]` markers and time budget | Future pacing signal in Xiaojiao in-class support |
| Student understanding/attention/frustration tracker | Future simulation-only diagnostic, not a real student profile |
| Activity categories and quiet/dialogue/discussion behavior | Future classroom rehearsal and time feasibility check |
| Prep outputs: `教案.md`, `说课稿.md`, `PPT脚本.md`, `课堂时间线.md`, `教材分析.md` | Future artifact chain, but only after source and teacher gate |

## Xiaojiao Direction

The later Xiaojiao execution line can be:

```text
single_lesson_template
-> teacher_execution_map
-> classroom_timeline
-> big_screen_pages
-> Xiaojiao in-class support
```

R250 should not turn this into runtime now. The correct next value is a contract for what `teacher_execution_map` and `classroom_timeline` must contain.

## Guardrails

- Do not import CrewAI/AutoGen/Chroma/Ollama dependencies into the main project now.
- Do not run classroom simulation against real teacher or student data.
- Do not treat simulated student state as persisted learner analytics.
- Do not bind PPT/big-screen pages before R230 has a surface contract.
- Do not let Xiaojiao auto-modify the lesson body; it can suggest pacing and confirmation items only after review gates exist.

