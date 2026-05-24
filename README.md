
# mmquotes

A personally curated collection of quotes organized by theme — primarily around leadership, resilience, discipline, strategy, and the mindset of operators and warfighters.  Built in JSON to import into various applications

## Structure

Each entry in `quotes.json` follows this schema:

```json
{
  "quote": "The text of the quote.",
  "author": "First Last",
  "category": "leadership | resilience | strategy | discipline | etc."
}
```

## Usage

[How you consume this — GitHub Action, script, API call, etc.]


## Schema

```json
{
  "quote": "string",
  "author": "string",
  "category": "string",
  "source": "string (optional — book, speech, interview)"
}
```

## Categories

| Tag | Description |
|-----|-------------|
| `leadership` | Command, accountability, people |
| `resilience` | Adversity, recovery, persistence |
| `discipline` | Process, habits, excellence |
| `strategy` | Planning, threat thinking, decision-making |
| `mentoring` | Development, growth, legacy |
| `warrior` | Military, warfighter, stoic tradition |

## How It's Used

[Brief description — e.g., "Rotated daily via GitHub Action into profile README" or "Consumed by a terminal tool built in Rust"]

## Contributing

This is a personal library. PRs not accepted, but feel free to fork.
