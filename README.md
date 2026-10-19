# AI Skills (`Arthur-Barreto/ai-skills`)

Custom AI agent skills and composite workflows created by Arthur Barreto for Claude Code, Cursor, Codex, and OpenClaw/omp.

## Authored Skills

| Skill | Description |
|---|---|
| [`linkedin-master-overhaul`](skills/linkedin-master-overhaul/SKILL.md) | 4-phase LinkedIn profile overhaul workflow combining automatic PDF intake (`Profile.pdf` + resume), design-tree grilling, de-AI-ified first-person copywriting, and bilingual (`EN` / `PT-BR`) step-by-step 10/10 execution guides. |

## Credits & Companion Skills Referenced

`linkedin-master-overhaul` is designed to orchestrate alongside and build upon these community skills (install them directly from their original authors):

- **[`mattpocock/skills`](https://github.com/mattpocock/skills)** by Matt Pocock — `grilling` (design-tree interview methodology) and `writing-for-agents` (skill design patterns).
- **[`BrianRWagner/ai-marketing-skills`](https://github.com/BrianRWagner/ai-marketing-skills)** by Brian Wagner — `linkedin-profile-optimizer` (section scoring rubric and AI search visibility framework).
- **`de-ai-ify`** by theflohart — AI pattern removal and natural human voice calibration.
- **[`paramchoudhary/resumeskills`](https://github.com/paramchoudhary/resumeskills)** by Param Choudhary — `resume-quantifier` and `resume-bullet-writer`.

### Installing Companion Skills

```bash
npx skills add mattpocock/skills
npx skills add brianrwagner/ai-marketing-claude-code-skills
npx skills add paramchoudhary/resumeskills
```

### Installing This Repository

```bash
npx skills add Arthur-Barreto/ai-skills
```
