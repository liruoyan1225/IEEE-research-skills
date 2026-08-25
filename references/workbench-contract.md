# Workbench contract

## Principle

Keep user-readable Markdown as the canonical working record and `project_index.json` as the machine-readable summary. A workbench may render or update the index, but must not overwrite confirmed Markdown decisions without creating a corresponding record.

## Required index fields

```json
{
  "schema_version": "1.0",
  "project": {"name": "", "scope": "", "target_venue": ""},
  "current": {"node": "", "deliverable": "", "status": "proposed"},
  "style_profile": {"default": "吕老师", "status": "confirmed"},
  "pending_confirmations": [],
  "confirmed_decisions": [],
  "trace_links": [],
  "versions": [],
  "blockers": []
}
```

## Status values

Use only `proposed`, `confirmed`, `rejected`, or `superseded`. Each record needs an ID, date, concise description, source paths, and an optional predecessor ID.

## Trace links

Use a link object to connect a claim, evidence card, equation, code revision, configuration, figure, manuscript location, comment, or review item. Store relative paths so a project directory remains portable.

## Workbench behavior

Display the current node, next deliverable, pending confirmations, blockers, and latest version by default. Reveal trace links, decision history, and profile evidence on demand. Require an explicit confirmation action before changing a record from `proposed` to `confirmed`.
