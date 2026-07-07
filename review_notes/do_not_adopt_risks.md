# Do Not Adopt Risks

## Hard No For Current Chain

- Do not copy Claw-ED code into R95, R201, R220, R210, or provider/runtime layers.
- Do not copy saniales GPL-3.0 code, agents, scripts, or templates into Xiaobei.
- Do not connect classmin CrewAI/AutoGen/Chroma/Ollama stack to Xiaobei mainline.
- Do not turn Divanshi Streamlit demo into Xiaobei UI.
- Do not let any external project write database, Feishu, memory store, formal export, or lesson baseline.
- Do not let external project concepts override `single_lesson_template`, source policy, teacher review gate, or R220F readonly route binding.

## Specific Risks

| Risk | Source | Why it matters | Mitigation |
| --- | --- | --- | --- |
| Bundle-first generation | Claw-ED | Can skip source ledger and teacher review if adopted too early | Use only as future output-chain reference |
| Broad runtime surface | Claw-ED | Includes provider calls, local writes, browser, Drive, Telegram, scheduler, package-install-like capabilities | Capability-level classification before reuse |
| GPL-3.0 license | saniales | Direct copying can contaminate licensing | Re-express ideas independently |
| Heavy agent stack | classmin | CrewAI/AutoGen/Chroma/Ollama expands dependencies and runtime risk | Keep as design reference |
| Simulated student data confusion | classmin | Simulation state could be mistaken for real learner analytics | Mark simulation-only and non-persistent |
| Hardcoded key pattern and old OpenAI dependency | Divanshi | Unsafe provider handling and stale SDK pattern | Use only field schema reference |
| Mainline distraction | All | R201/R220 still need stability | Freeze R250 as docs-only |

## Review Gate

Before any follow-up implementation task claims to adopt these references, it must state:

```text
Which idea is adopted?
Which source repo inspired it?
Is any code copied? If yes, stop.
Which Xiaobei stage owns it?
What is the no-write/no-provider/no-formal-apply boundary?
What is the rollback path?
```

