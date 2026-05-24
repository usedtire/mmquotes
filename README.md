# mmquotes

A personally curated collection of quotes organized by theme — primarily around leadership, resilience, discipline, strategy, and the mindset of operators and warfighters. Built in JSON for easy consumption by scripts, actions, or tools.

## Schema

Each entry in `quotes.json` follows this structure:

```json
{
  "quote": "string",
  "author": "string",
  "category": "string",
  "tags": ["array", "of", "strings"],
  "time_of_day": "morning | afternoon | evening | anytime",
  "source": "string (optional — book, speech, interview)"
}
```

`tags` and `time_of_day` are optional. `source` is omitted when unknown.

## Categories

| Tag | Description |
|-----|-------------|
| `leadership` | Command, accountability, people |
| `resilience` | Adversity, recovery, persistence |
| `discipline` | Process, habits, excellence |
| `strategy` | Planning, threat thinking, decision-making |
| `mentoring` | Development, growth, legacy |
| `warrior` | Military, warfighter, stoic tradition |
| `cybersecurity` | Threat mindset, defense, operational security |

## Contributing

This is a personal library. PRs not accepted, but feel free to fork.
