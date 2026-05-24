# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A personal quotes library (`quotes.json`) — a single JSON file with a top-level `quotes` array. No build system, no dependencies, no tests.

## Schema

Every entry in `quotes.json` follows this structure:

```json
{
  "quote": "string (required)",
  "author": "string (required)",
  "category": "string (required — see valid values below)",
  "tags": ["array", "of", "strings (optional)"],
  "time_of_day": "morning | afternoon | evening | anytime (optional)",
  "source": "string (optional — book, speech, interview)"
}
```

### Valid `category` values

`leadership`, `resilience`, `discipline`, `strategy`, `mentoring`, `warrior`, `cybersecurity`

### `tags` vs `category`

`category` is the primary classification (one value). `tags` is a broader array that can overlap with other categories — a quote can have `"category": "warrior"` and `"tags": ["warrior", "resilience", "strategy"]`.

## Editing quotes.json

After any edit, validate the JSON is well-formed:

```bash
python3 -m json.tool quotes.json > /dev/null && echo "valid"
```

## Style conventions

- Quotes are the exact original text — no paraphrasing.
- `author` is "First Last" format (e.g., `"Marcus Aurelius"`, not `"Marcus Aurelius, Roman Emperor"`).
- `source` is omitted when unknown, not left as an empty string.
- `time_of_day` is omitted when the quote has no natural morning/evening resonance.
