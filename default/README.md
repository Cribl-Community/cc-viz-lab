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
| **Charts** | **103** built-in visualizations (listed below) + plugin gallery + your own plugins |
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
| **KQL Explainer** | Paste a KQL query and get an annotated version with `//` comments explaining each pipe stage above the original KQL line (Cribl AI when connected, heuristic otherwise) |
| **Dataset Mapper** | Map legacy source names (Splunk indexes, Sumo partitions, etc.) to Cribl dataset names; auto-substitute in any pasted query |
| **Tracker** | Track migration item status, blockers, and progress; export as Markdown or executive summary |
| **Readiness Report** | One-click scored audit of all dashboards and saved searches — produces issues, recommendations, and a dataset inventory |

---

## Built-in visualizations (103)

Viz Lab ships with **103 visualizations** across 7 categories. **+ Plugins** can add more from the gallery or custom ESM URLs.

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

### Gallery — ECharts Extended (21)

Theme River, Pictorial Bar, Wind Rose, Polar Scatter, Liquid Fill, **Nightingale Rose**, **Bar Race**, **Circular Graph**, **Sankey (Vertical)**, **3D Gauge**, **3D Funnel**, **3D Pie**, **Stacked Donut**, **Calendar Scatter**, **Radar (Polar)**, **Bubble Map**, **River Flow**, **Polar Bar**, **3D Globe (ECharts)**, **3D Scatter (ECharts)**

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

### Gallery — D3 (16)

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

### Gallery — Chart.js (9)

Bubble, Mixed, Polar Area, Radar, Scatter, Stacked Bar, **Nested Doughnut**, **Stacked Area**, **Floating Bar**, **Timeline**

![Nested Doughnut](../docs/images/viz/g-doughnut-nested.png)
![Stacked Area](../docs/images/viz/g-area-stacked.png)
![Floating Bar](../docs/images/viz/g-floating-bar.png)
![Timeline](../docs/images/viz/g-timeline.png)

---

## Plugins (optional)

Open **+ Plugins** on Search → install from the gallery or paste a **trusted** ESM URL / file. Plugin code runs with full page permissions—only load sources you trust.

---

## Need developer docs?

The install bundle is the runnable app. Full repository documentation (architecture, tests, parity notes, **dashboard and search converters**, Plain English → KQL) lives in the root **README.md** and **docs/** of the **source repo**, not in this file.
