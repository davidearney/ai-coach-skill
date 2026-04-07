# ai-coach-skill

A personal AI learning coach for [Claude Code](https://claude.ai/code). Helps you build deep, practical competency with GenerativeAI, Agentic AI, and the modern AI tooling ecosystem.

## Install

```bash
claude skill install https://github.com/davidearney/ai-coach-skill
```

Or manually copy `SKILL.md` to `~/.claude/skills/ai-coach/SKILL.md`.

## Usage

```
/ai-coach                        # show status and learning path
/ai-coach assess                 # knowledge assessment to calibrate your level
/ai-coach lesson                 # next lesson in your learning path
/ai-coach lesson tokens          # lesson on a specific topic
/ai-coach lessons                # list all lessons with completion status
/ai-coach quiz                   # quiz on most recent lesson
/ai-coach quiz tool-use          # quiz on a specific topic
/ai-coach progress               # full progress report
/ai-coach update                 # pull latest skill from GitHub
/ai-coach what is RAG?           # ask anything about AI
```

## What it does

- **Assesses your knowledge** across LLM fundamentals, prompting, agentic AI, building with AI, and the AI landscape
- **Builds a personalized learning path** — three curriculum stages based on your level
- **Delivers structured lessons** with framing, mechanics, practical examples, and comprehension checks
- **Quizzes you** with practical questions focused on understanding, not trivia
- **Tracks your progress** across sessions in `progress/profile.md` and daily session logs

## Curriculum

| Domain | Lessons |
|--------|---------|
| LLM Fundamentals | `tokens`, `context`, `temperature`, `models` |
| Prompt Engineering | `system-prompts`, `few-shot`, `chain-of-thought`, `structured-output` |
| Agentic AI | `agentic-basics`, `tool-use`, `mcp`, `multi-agent` |
| Claude API | `claude-api`, `sdk-patterns` |
| Building AI Apps | `rag-basics`, `embeddings` |
| Claude Code | `claude-code-advanced` |
| AI Quality | `evals` |
| AI Safety | `ai-safety` |

## Progress tracking

The skill stores progress in a `progress/` directory relative to where your learning repo lives. The profile path is configured in `SKILL.md` — update it to match your local setup.

- `progress/profile.md` — knowledge levels, learning path, preferences
- `progress/YYYY-MM-DD.md` — daily session logs

## Updating

In-session:
```
/ai-coach update
```

Or pull manually and copy `SKILL.md` to `~/.claude/skills/ai-coach/SKILL.md`.

## Customizing

`SKILL.md` is the skill prompt — edit it directly to:
- Add new lesson topics
- Adjust the coaching persona
- Change progress file paths
- Add your own background context

The skill is loaded fresh each session, so edits take effect immediately.

## License

MIT
