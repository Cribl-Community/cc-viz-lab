# Viz Lab — what it does

**Viz Lab** is a **Cribl Search** app. Run **KQL**, browse **Events** and **Fields**, pick a **Chart**, and build **Dashboards** with drag-and-drop panels — in grid or free-form **Canvas** layout. There is no separate "Data" hub here—use native Cribl Search for dataset administration if you need it.

---

## Quick use

1. **Search** — Write KQL (or use Plain English if Copilot is available), set the **time range**, click **Search**.
2. Open **Events** (raw rows), **Fields** (column stats), or **Chart** (pick a visualization on the right).
3. Map your result columns to the chart's channels (dropdowns at the top of the viz panel). Use the small **chart icon** beside a viz name to load a **sample query** for that chart; then click **Search** again to run it.
4. **Dashboards** — Create grids of panels, variables, tabs, and imports (Splunk XML/Studio, Sumo, Kibana, Grafana, Cribl JSON, Viz Lab JSON). Choose **Grid** or **Canvas** (free-form absolute positioning) layout when creating a new dashboard. Use **+ Plugins** to add extra charts from the gallery or a URL.

---

## Features (short)

| Area | What you get |
|------|----------------|
| **Search** | KQL editor, time picker, sampling, history, saved searches, CSV/NDJSON export, optional streaming rows, annotations |
| **Charts** | **55** core + **49** gallery = **104** built-in visualizations (listed below) + your own plugins |
| **Dashboards** | Grid and Canvas layout modes, parent/child searches, variables, versions, collaboration (when configured), export. Dashboard list shows a Grid/Canvas layout column with sidebar filter |
| **Converters** | Dashboard import from **5 sources** (Splunk SimpleXML, Splunk Dashboard Studio, Sumo Logic, Kibana, Grafana). Query translator covers **7 languages** (SPL, ES\|QL, LogQL, Sumo Logic, Kibana KQL, SQL, Sigma) to Cribl KQL |
| **Knowledge** | In-app shortcuts to lookups, parsers, regexes, grok, macros (same API as Search) |
| **Performance** | Real-time search execution metrics, per-run timing, P95, snapshots, before/after comparison |
| **AI** | Wiz Viz chat assistant, Investigate agent, Query Studio AI generation, LLM Skills library |
| **Security** | Investigations timeline, Hunt Board (PEAK), IOC Lookup, Anonymizer |
| **Theme** | Light/dark follows Cribl when embedded; manual override in standalone use |

---

## Sidebar — 30+ productivity & workspace tools

All tools are accessible from the left sidebar (grouped into collapsible sections) and the command palette.

### Search Home

| Tool | What it does |
|------|--------------|
| **Run a search** | KQL editor with Plain English, time picker, Events/Fields/Chart tabs |

### History

| Tool | What it does |
|------|--------------|
| **History** | Browse and re-run previous searches |

### Saved Searches

| Tool | What it does |
|------|--------------|
| **All saved searches** | List, filter, and manage saved searches and collections |
| **Search Converter** | Convert saved searches from Splunk SPL and other formats to Cribl KQL |

### Dashboards

| Tool | What it does |
|------|--------------|
| **All dashboards** | List with Grid/Canvas layout column, collection filter, tags, sort |
| **Dashboard Converter** | Import dashboards from 5 sources: Splunk SimpleXML, Splunk Dashboard Studio, Sumo Logic, Kibana, Grafana |
| **Dashboard Templates** | Start a new dashboard from a curated blueprint; save any dashboard as a custom template |
| **Export for Cribl** | Convert a Viz Lab dashboard to Cribl wire JSON with a per-panel status report; push directly to a connected tenant |
| **Bulk Export ZIP** | Select multiple dashboards and download them as a ZIP of Cribl JSON files |
| **Health Check** | Scan every dashboard for blank panels, missing variables, orphaned parent refs, and empty query variables |

### Utilities — Search & Query

| Tool | What it does |
|------|--------------|
| **Query Studio** | Unified workspace: Library (snippets + templates) / Explain & Format / Diff & Optimize / Translate — one tabbed view |
| **Query Translator** | 7-language translator: SPL, ES\|QL, LogQL, Sumo Logic, Kibana KQL, SQL, Sigma to Cribl KQL |

### Utilities — Data & Knowledge

| Tool | What it does |
|------|--------------|
| **Field Profiler** | Sample any dataset and get a full field-type, presence-rate, and sample-value breakdown. Auto-populates the dataset dropdown from your tenant's catalog |
| **Dataset Mapper** | Map legacy source names (Splunk indexes, Sumo partitions, etc.) to Cribl dataset names; auto-substitute in any pasted query |
| **Knowledge** | In-app shortcuts to lookups, parsers, regexes, grok, macros (same API as Search) |
| **Lookup Manager** | Browse, create, edit, and test lookup tables used by the `lookup` operator |

### Utilities — Security & Ops

| Tool | What it does |
|------|--------------|
| **Investigations** | Timeline-based incident tracking with hypotheses (confidence levels), findings, query log, Hunt Board (PEAK kanban), and IOC Lookup (Shodan, AbuseIPDB, VirusTotal, GreyNoise) |
| **Anonymizer** | Redact IPs, emails, credentials, PII from logs before sharing with support or AI tools |
| **Run Book** | Operational procedures with numbered KQL steps; run each step directly in Search |

### Utilities — AI & Automation

| Tool | What it does |
|------|--------------|
| **Wiz Viz** | AI-powered assistant — write KQL, design dashboards, hunt threats, get architecture advice; includes LLM Skills library |

### Utilities — Migration

| Tool | What it does |
|------|--------------|
| **Tracker** | Track migration item status, blockers, and progress; export as Markdown or executive summary |

### Utilities — Workspace

| Tool | What it does |
|------|--------------|
| **Productivity Hub** | App-state snapshots (backup/restore) and workflow recordings |
| **Usage Dashboard** | Personal analytics — searches run, daily activity, datasets, feature adoption |
| **Whiteboard** | Interactive Cribl architecture diagram (Sources → Stream → Destinations) with value stories |
| **Theme Builder** | Create and save custom color palettes for dashboard visualizations |
| **Demos & Training** | Build demo scenarios with vendor templates (Palo Alto, CrowdStrike, CloudTrail, K8s, Okta) |
| **Performance Metrics** | Every search execution logged with ms timestamps, run grouping, P95, snapshots, export |
| **Diagnostics** | One-click health check: API connectivity, storage, environment; exportable report |

### App-level

| Tool | What it does |
|------|--------------|
| **App settings** | Global preferences, API connection, feature flags |
| **Customize sidebar** | Toggle sections on/off; hidden items remain in the command palette |
| **Packs** | Link to native Cribl Packs |
| **Help** | In-app user guide and keyboard shortcuts |

---

## Built-in visualizations (104)

Viz Lab ships with **104 visualizations** across 7 categories. **+ Plugins** can add more from the gallery or custom ESM URLs.

### Basic Charts (24)

Column, Horizontal Bar, Radial Bar, Line, Bump Chart, Area, Pie, Donut, Scatter, Bubble, Single Value, Arc Gauge, Table, Events, KPI Strip, Radial Gauge, Marker Gauge, Speedometer Gauge, Liquid Fill Gauge, Linear Gauge, Honeycomb Status, App Status Tiles, Status Grid, Funnel

![Column chart](../docs/images/viz/column.png)
![Pie chart](../docs/images/viz/pie.png)
![Funnel](../docs/images/viz/funnel.png)

### Statistical & Time-Series (9)

Heatmap, Box Plot, Parallel Coordinates, Calendar Heatmap, Candlestick, Waterfall, Dumbbell, Bullet, Gantt

![Heatmap](../docs/images/viz/heatmap.png)
![Waterfall](../docs/images/viz/waterfall.png)
![Calendar](../docs/images/viz/calendar.png)

### Networks & Hierarchies (7)

Sankey, Network Graph, Chord Diagram, Flow Diagram (React Flow), Tree / Dendrogram, Treemap, Sunburst

![Network](../docs/images/viz/network2d.png)
![Treemap](../docs/images/viz/treemap.png)
![Sunburst](../docs/images/viz/sunburst.png)

### Geo & 3D (8)

Isometric Bars, 3D Scatter, 3D Surface, 3D Network, Geo Choropleth, Globe (Three.js)

![Geo Choropleth](../docs/images/viz/geo-choropleth.png)

### Security (9)

MITRE ATT&CK Matrix, Cyber Kill Chain Funnel, Detection Coverage Radar, Process Lineage Tree, Attack Path Graph, Auth Anomaly Heatmap, Geo Attack Flows, Alert Correlation, IOC Velocity Streamgraph

![MITRE Matrix](../docs/images/viz/mitre-matrix.png)
![Detection Radar](../docs/images/viz/detection-radar.png)

### Gallery — ECharts Extended (22)

Theme River, Pictorial Bar, Wind Rose, Polar Scatter, Liquid Fill, **Nightingale Rose**, **Bar Race**, **Circular Graph**, **Sankey (Vertical)**, **3D Gauge**, **3D Funnel**, **3D Pie**, **Stacked Donut**, **Calendar Scatter**, **Radar (Polar)**, **Bubble Map**, **River Flow**, **Polar Bar**, **3D Globe (ECharts)**, **3D Scatter (ECharts)**, **Radar Spider**, **Ring Gauge**

![Nightingale Rose](../docs/images/viz/g-nightingale.png)
![Bar Race](../docs/images/viz/g-bar-race.png)
![Sankey Vertical](../docs/images/viz/g-sankey-vertical.png)
![Donut Stack](../docs/images/viz/g-donut-stack.png)
![Radar Polar](../docs/images/viz/g-radar-polar.png)
![Polar Bar](../docs/images/viz/g-polar-bar.png)
![River Flow](../docs/images/viz/g-river.png)
![3D Funnel](../docs/images/viz/g-funnel-3d.png)
![3D Pie](../docs/images/viz/g-pie-3d.png)
![3D Gauge](../docs/images/viz/g-gauge-3d.png)

### Gallery — D3 (17)

Force Bubbles, Hexbin, Radial Tree, Streamgraph, Word Cloud, Zoomable Sunburst, **Violin Plot**, **Beeswarm**, **Lollipop Chart**, **Arc Diagram**, **Packed Circles**, **Ridgeline Plot**, **Slope Chart**, **Waffle Chart**, **Dot Plot**, **Histogram**, **Marimekko**

![Violin Plot](../docs/images/viz/g-violin.png)
![Beeswarm](../docs/images/viz/g-beeswarm.png)
![Lollipop](../docs/images/viz/g-lollipop.png)
![Arc Diagram](../docs/images/viz/g-arc-diagram.png)
![Packed Circles](../docs/images/viz/g-packed-circles.png)
![Ridgeline](../docs/images/viz/g-ridgeline.png)
![Slope Chart](../docs/images/viz/g-slope-chart.png)
![Waffle](../docs/images/viz/g-waffle.png)
![Dot Plot](../docs/images/viz/g-dot-plot.png)
![Histogram](../docs/images/viz/g-histogram.png)
![Marimekko](../docs/images/viz/g-marimekko.png)

### Gallery — Chart.js (10)

Bubble, Mixed, Polar Area, Radar, Scatter, Stacked Bar, **Nested Doughnut**, **Stacked Area**, **Floating Bar**, **Timeline**

![Nested Doughnut](../docs/images/viz/g-doughnut-nested.png)
![Stacked Area](../docs/images/viz/g-area-stacked.png)
![Floating Bar](../docs/images/viz/g-floating-bar.png)
![Timeline](../docs/images/viz/g-timeline.png)

---

## Workspace & productivity tools

![Search home with datasets, history, and visualization picker](../docs/images/search-home.png)

![Performance Metrics — KPI strip, run grouping, heatmap durations](../docs/images/search-performance.png)

![Query Studio — snippets, explain, format, translate](../docs/images/query-studio.png)

![Whiteboard — interactive Cribl architecture diagram](../docs/images/whiteboard.png)

![Scaffold — guided wizard to build a whole dashboard from Markdown](../docs/images/scaffold.png)

![Investigations — Timeline, Hunt Board, IOC Lookup](../docs/images/investigations.png)

![Wiz Viz — conversational AI assistant](../docs/images/wiz-viz.png)

![Productivity Hub — snapshots and recordings](../docs/images/productivity-hub.png)

---

## Plugins (optional)

Open **+ Plugins** on Search → install from the gallery or paste a **trusted** ESM URL / file. Plugin code runs with full page permissions—only load sources you trust.

---

## Need developer docs?

The install bundle is the runnable app. Full repository documentation (architecture, tests, parity notes, **dashboard and search converters**, Plain English → KQL) lives in the root **README.md** and **docs/** of the **source repo**, not in this file.
