# Viz Lab — what it does

**Viz Lab** is a **Cribl Search** app. Run **KQL**, browse **Events** and **Fields**, pick a **Chart**, and build **Dashboards** with drag-and-drop panels. There is no separate "Data" hub here—use native Cribl Search for dataset administration if you need it.

---

## Quick use

1. **Search** — Write KQL (or use Plain English if Copilot is available), set the **time range**, click **Search**.
2. Open **Events** (raw rows), **Fields** (column stats), or **Chart** (pick a visualization on the right).
3. Map your result columns to the chart's channels (dropdowns at the top of the viz panel). Use the small **chart icon** beside a viz name to load a **sample query** for that chart; then click **Search** again to run it.
4. **Dashboards** — Create grids of panels, variables, tabs, and imports (Splunk XML, Cribl JSON, Viz Lab JSON). Use **+ Plugins** to add extra charts from the gallery or a URL.

---

## Features (short)

| Area | What you get |
|------|----------------|
| **Search** | KQL editor, time picker, sampling, history, saved searches, CSV/NDJSON export, optional streaming rows, annotations |
| **Charts** | **55** built-in visualizations (listed below) + plugin gallery + your own plugins |
| **Dashboards** | Layout editor, parent/child searches, variables, versions, collaboration (when configured), export |
| **Knowledge** | In-app shortcuts to lookups, parsers, regexes, grok, macros (same API as Search) |
| **Theme** | Light/dark follows Cribl when embedded; manual override in standalone use |

---

## Migration & productivity tools

These tools live in the sidebar and are designed to help teams migrate from other platforms to Cribl Search.

| Tool | What it does |
|------|--------------|
| **Dashboard Templates** | Start a new dashboard from a curated blueprint; save any dashboard as a custom template |
| **Export for Cribl** | Convert a Viz Lab dashboard to Cribl wire JSON with a per-panel status report; push directly to a connected tenant |
| **Bulk Export ZIP** | Select multiple dashboards and download them as a ZIP of Cribl JSON files |
| **Dashboard Health Check** | Scan every dashboard for blank panels, missing variables, orphaned parent refs, and empty query variables |
| **Field Profiler** | Sample any dataset and get a full field-type, presence-rate, and sample-value breakdown. Auto-populates the dataset dropdown from your tenant's catalog |
| **Query Library** | 24 curated KQL snippets for security, infrastructure, application, network, and compliance use cases |
| **KQL Formatter** | Pretty-print or minify a KQL query — one pipe stage per line, indented subqueries |
| **KQL Explainer** | Paste a KQL query and get a plain-English explanation of each pipe stage (Cribl AI when connected, heuristic otherwise) |
| **Dataset Mapper** | Map legacy source names (Splunk indexes, Sumo partitions, etc.) to Cribl dataset names; auto-substitute in any pasted query |
| **Tracker** | Track migration item status, blockers, and progress; export as Markdown or executive summary |
| **Readiness Report** | One-click scored audit of all dashboards and saved searches — produces issues, recommendations, and a dataset inventory |

---

## Built-in visualizations (55)

These ship with the app. **+ Plugins** can add more.

**Basic** — Column, Horizontal Bar, Line, Area, Pie, Donut, Scatter, Single value, Arc Gauge, Table, Events, KPI Strip, Radial Gauge, Marker Gauge, Speedometer Gauge, Liquid Fill Gauge, Linear Gauge, Honeycomb Status, App Status Tiles, Status Grid, Funnel

**Statistical & time-series** — Heatmap, Boxplot, Parallel Coordinates, Calendar Heatmap, Candlestick, Waterfall, Bullet, Gantt

**Networks & hierarchies** — Sankey, Network Graph, Chord Diagram, Flow Diagram, Tree (Dendrogram), Treemap, Sunburst

**Geo & 3D** — Isometric Bars, 3D Scatter, 3D Network, Geo Choropleth

**Security** — MITRE ATT&CK Matrix, Cyber Kill Chain, Detection Coverage Radar, Process Lineage, Attack Path Graph, Auth Anomaly Heatmap, Geo Attack Flows, Alert Correlation, IOC Velocity

---

## Plugins (optional)

Open **+ Plugins** on Search → install from the gallery or paste a **trusted** ESM URL / file. Plugin code runs with full page permissions—only load sources you trust.

---

## Need developer docs?

The install bundle is the runnable app. Full repository documentation (architecture, tests, parity notes, **dashboard and search converters**, Plain English → KQL) lives in the root **README.md** and **docs/** of the **source repo**, not in this file.
