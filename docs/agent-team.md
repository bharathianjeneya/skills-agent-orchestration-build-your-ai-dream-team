# Agent team

For Mona's Project Pulse dashboard, I will use a four-agent custom team orchestrated with GitHub Copilot CLI in a Codespace. Each agent is defined in the repository's agent folder and assigned a specialist role for planning, coordination, implementation, and design.

- Planner — Model: Claude Opus 4.7 (copilot) — Definition: .github/agents/planner.agent.md — Researches the repo and requirements, identifies dependencies and edge cases, and produces the implementation plan that the team will execute.
- Orchestrator — Model: Claude Opus 4.7 (copilot) — Definition: .github/agents/orchestrator.agent.md — Breaks the plan into phases, delegates work to specialists, manages sequencing, and checks that the integrated result fits together.
- Coder — Model: GPT-5.5 (copilot) — Definition: .github/agents/coder.agent.md — Implements app logic, fixes bugs, writes supporting configuration when required, and validates changes within the assigned file scope.
- Designer — Model: Gemini 3.1 Pro (copilot) — Definition: .github/agents/designer.agent.md — Focuses on UI/UX, accessibility, visual hierarchy, interaction flow, and the polished dashboard experience for Project Pulse.

This workflow uses GitHub Copilot CLI in a Codespace to coordinate the Planner, Orchestrator, Coder, and Designer as a single delivery team.
