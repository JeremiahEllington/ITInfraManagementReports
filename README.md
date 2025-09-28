# IT Infrastructure Management Reports

Concise, standardized templates for infrastructure operations, security, capacity, cost, risk, and governance reporting.

## Goals
- Consistency: common structure & terminology
- Velocity: ready-to-fill templates, minimal rework
- Traceability: clear data source + KPI definitions
- Actionability: highlight decisions, blockers, ownership

## Structure
```
/operations
/security
/capacity
/financial
/governance
/shared
```

## Template Front-Matter (YAML)
```yaml
report: Incident Summary
period: 2025-09-01..2025-09-30
owner: ops-lead
status: draft
version: 1.0
last_updated: 2025-09-28
kpis: [ MTTR, IncidentCount, Sev1Count ]
```

## Core Files (Planned)
- REPORT_CATEGORIES.md – scope & audience per category
- KPI_DEFINITIONS.md – canonical KPI names & formulas
- DATA_SOURCES.md – systems + extraction cadence
- SCHEDULE_GUIDE.md – reporting calendar
- AUTOMATION_GUIDE.md – script generation patterns

## Usage (Short)
1. Pick template closest to need
2. Copy to date folder (`YYYY-MM` or week number)
3. Fill KPI section referencing definitions
4. Add action items with owner + due date
5. Commit; open review PR if executive-facing

---
Small, composable. No slide decks unless necessary.
