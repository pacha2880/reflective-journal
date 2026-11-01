# reflective-journal

A Claude skill that turns a conversation into a reflective personal journal, in any language.

You write entries the way you would in a diary, with a date and place if you like, and Claude reads them, responds with warmth and honesty, notices emotions and patterns over time, connects them to your goals, and closes each entry with a verified Stoic quote and two reflective questions.

It is not a productivity system and not a substitute for therapy. It is meant to help you observe yourself, recognize your progress, and decide with more awareness.

## What it does

- **Responds in your language.** The instructions are in English, but replies follow the language and regional variety you write in, or the one your profile asks for.
- **Keeps continuity.** Entries in the same chat are treated as one journal; people, decisions and open threads carry over.
- **Readable replies.** A dated header, short paragraphs, light structure for long entries, shorter replies for short entries.
- **Stoic quotes you can trust.** A base bank of quotes from Epictetus, Seneca and Marcus Aurelius with work and passage references, rendered into your language and labeled as free translation or paraphrase. Other passages are allowed only when their source is certain; known fake attributions are listed to avoid.
- **Asides.** Write "aside" (or "paréntesis", or a keyword you define) to ask something outside the journal, then continue.
- **Pasted texts stay journal content.** Meeting notes or messages you wrote are reflected on, not edited, unless you ask.
- **Careful with hard moments.** Self-compassion when you're harsh on yourself, grounding for anxiety, no diagnoses, and a dedicated response when there are risk signals.
- **Summaries.** Ask for a summary or extraction of the journal and get a chronological review with patterns and open threads.

## Install

### As a Claude Code plugin

```
/plugin marketplace add pacha2880/reflective-journal
/plugin install reflective-journal@reflective-journal
```

### As a standalone skill

Copy `skills/reflective-journal/` into your skills directory (for Claude Code, `~/.claude/skills/reflective-journal/`), or upload the folder as a skill in Claude.

## Your profile (optional)

Copy `skills/reflective-journal/references/profile-template.md` to a `profile.md`, fill it in, and paste or attach it at the start of your journal chat. It tells Claude your name, language, current goals, goals already reached, and the people who come up often.

Keep your profile out of version control. This repo's `.gitignore` already ignores `profile.md` and `profile-*.md`.

## Structure

```
.claude-plugin/
  plugin.json
  marketplace.json
skills/reflective-journal/
  SKILL.md
  references/
    stoic-quotes.md
    profile-template.md
```

## Credits

Ideas drawn from Seneca's evening examination (*On Anger* III.36), Kristin Neff's self-compassion journal, and James Pennebaker's research on expressive writing.

## License

MIT

---

## En español

Una skill de Claude que convierte una conversación en un diario personal reflexivo, en cualquier idioma. Escribes tus entradas como en un diario y Claude las comenta con calidez y honestidad, detecta patrones, las conecta con tus objetivos y cierra cada entrada con una cita estoica verificada y dos preguntas. Las instrucciones están en inglés para que se pueda compartir, pero responde en el idioma en que escribas. Para personalizarla, llena la plantilla de perfil y pégala al inicio de tu chat del diario.
