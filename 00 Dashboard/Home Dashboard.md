# Home Dashboard

## Current Focus
- [[01 AI & Development/AI Development System]]
- [[02 Work Architecture/OCE CMA Context Engine]]
- [[03 Home & Move/Move Plan]]
- [[04 Bible & Theology/Bible Study System]]
- [[05 Investing/Investing Dashboard]]

## Quick Capture
Use [[00 Dashboard/Inbox]] for anything not yet organized.

## Active Decisions
```dataview
LIST
FROM ""
WHERE contains(file.tags, "#decision")
SORT file.mtime desc
```

## Active Projects
```dataview
LIST
FROM ""
WHERE contains(file.tags, "#project") AND contains(file.tags, "#active")
SORT file.mtime desc
```

## Review Rhythm
- Daily: capture tasks and decisions
- Weekly: review active projects, move logistics, finance/watchlist, learning goals
- Monthly: archive completed notes and update long-term strategy
