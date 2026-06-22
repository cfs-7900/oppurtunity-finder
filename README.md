# CFS Opportunity Finder — Dashboards

Public hosting for Camelot Facility Services (CFS) executive maintenance dashboards.

## Why this repo exists

This repository hosts a set of **self-contained, interactive HTML dashboards** built from
Camelot's CMMS work-order and asset data. They are published here via **GitHub Pages** so they
can be opened in any browser and **shared with stakeholders through a simple link** — no Power BI,
no server, no login, and no software to install.

The dashboards turn raw work-order exports into an executive view focused on the core question:
**where can Camelot generate revenue beyond the base maintenance contract** — by self-performing
work currently outsourced to vendors, recovering missed billing, and identifying project-bid
candidates — alongside running data-quality and SWOT insight.

Each page includes live Client / Database / Month filters, KPI cards, trend and breakdown charts,
auto-generated insights, and sortable detail tables. Every file is fully self-contained (all data
and charts are embedded — no external/CDN calls).

## Dashboards

| Dashboard | Link |
|---|---|
| Master Executive Dashboard | [Master Executive Dashboard](https://cfs-7900.github.io/oppurtunity-finder/index.html) |
| Opportunity Finder | [Opportunity Finder](https://cfs-7900.github.io/oppurtunity-finder/opportunity-finder.html) |
| Work Orders | [Work Orders](https://cfs-7900.github.io/oppurtunity-finder/work-orders.html) |
| Assets | [Assets](https://cfs-7900.github.io/oppurtunity-finder/assets.html) |
| Data Quality | [Data Quality](https://cfs-7900.github.io/oppurtunity-finder/data-quality.html) |

> Start with the **Master Executive Dashboard**, then use the in-page tabs to move between views.

## Coverage

Reporting period **January–December 2025** · 16,538 work orders · 21 clients across multiple CMMS
databases · 5,030 asset records.

## Updating

Dashboards are regenerated from source data by the project pipeline (`scripts/etl.py` then
`scripts/gen.py`) and the resulting HTML files in this repository are replaced. GitHub Pages
redeploys automatically on each push to `main`.
