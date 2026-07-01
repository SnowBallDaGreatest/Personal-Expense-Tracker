# Personal Expense Tracker — Sprint 3

Full-featured desktop expense tracker built with Python · Tkinter · SQLite / Firebase · Matplotlib · ReportLab

## Quick Start

```bash
pip install matplotlib reportlab
python main.py
```

## All Tabs

| Tab | Features |
|---|---|
| Dashboard | KPI cards, doughnut, 14-day line, Needs/Wants/Savings bar |
| + Add | Validated form, category group indicator |
| History | Filter/search/sort by month+category+group, edit, delete |
| Charts | Doughnut, monthly bar, stacked category x month, cumulative area |
| Summary | Heatmap calendar, category table, payment bars, month comparison |
| Budget | Monthly limits per category, visual progress bars |
| Recurring | Auto-post daily/weekly/monthly/yearly expenses on launch |
| Search | Live full-text search, autocomplete, chip filters, highlight |
| Categories | Full CRUD with colour picker, icon, group assignment |
| Export | CSV + PDF report with embedded charts |
| Import | CSV import with preview, validation, fuzzy category matching |
| Settings | Theme toggle, currency, backup/restore DB |

## File Structure

```
expense_tracker/
├── main.py                  App shell + tab orchestration
├── requirements.txt
├── core/
│   ├── database.py          All SQLite queries
│   ├── theme.py             All design tokens (retheme here)
│   └── exporter.py          CSV + PDF export engine
└── ui/
    ├── widgets.py           Reusable widgets
    ├── tab_dashboard.py
    ├── tab_add_expense.py
    ├── tab_history.py
    ├── tab_charts.py
    ├── tab_summary.py       [Sprint 3] Heatmap + payment breakdown
    ├── tab_budget.py
    ├── tab_recurring.py     [Sprint 3] Auto-recurring expenses
    ├── tab_search.py        [Sprint 3] Smart full-text search
    ├── tab_categories.py
    ├── tab_export.py
    ├── tab_import.py        [Sprint 3] CSV import
    └── tab_settings.py
```

## Agile Sprint Roadmap

| Sprint | Status | Features |
|--------|--------|---------|
| Sprint 1 | Done | Core CRUD, 4 charts, budgets, dark UI |
| Sprint 2 | Done | CSV/PDF export, settings, theme toggle, DB backup |
| Sprint 3 | Done | Recurring, summary heatmap, smart search, CSV import |
| Sprint 4 | Next | Receipt photo, voice input, AI categorisation |
