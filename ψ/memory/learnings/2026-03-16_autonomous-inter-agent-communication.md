# Autonomous Inter-Agent Communication: Lessons Learned

## Explicit Shell Mode for Agent Commands
When instructing another Gemini CLI agent to run a shell command via `tmux send-keys`, it's crucial to explicitly guide them into "shell mode" (`! shell`) first, then issue the command, and finally return them to "agent mode" (`! agent`). This bypasses the agent's natural language interpretation layer and ensures direct command execution.

## Shared Memory as a Robust Fallback
Shared memory (`ψ/`) provides a reliable, asynchronous channel for inter-agent communication. It's particularly effective when direct real-time interaction is complex, requires persistence, or is prone to interpretive ambiguity, serving as an excellent backup for real-time channels.

## Understanding Agent Interpretation
Different AI agents (even running the same CLI) may interpret inputs differently based on their current mode and internal logic. Effective communication protocols must meticulously account for these variations, often requiring explicit directives (like shell mode toggles) to ensure intended actions are performed. This highlights the importance of precise, unambiguous instructions in multi-agent systems.
