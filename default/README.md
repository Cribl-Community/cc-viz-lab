# Cribl Search Tools — what it does

**Cribl Search Tools** is a **Cribl Search** app. Run **KQL**, browse **Events** and **Fields**, pick a **Chart**, and build **Dashboards** — in grid or free-form **Canvas** layout. Everything is one or two clicks from the sidebar.

---

## Quick use

1. **Search** — Write KQL (or plain English), set the time range, click Search.
2. Switch between **Events** (rows), **Fields** (column stats), or **Chart** (pick any visualization).
3. **Save** your search or drop it into a **Dashboard** panel.
4. **Dashboards** — Grid or Canvas layout, variables, imports, collaboration.

Press **⌘K** (Ctrl+K) anytime to jump to any page, dashboard, saved search, or action.

---

## Sidebar

The sidebar uses expandable groups. Everything is also reachable via **⌘K** (Command Palette).

| Item | What you get |
|------|--------------|
| **Search** | New Search, Saved Searches, History, Knowledge (lookups/parsers/regex/grok/macros), Notebooks, Query Workbench |
| **Dashboards** | My Dashboards, Collections, Health, Diff, Snapshots |
| **Migrate** | Overview, Translate Queries, Convert Dashboards (9 vendors), Metrics Migration |
| **Utilities** | Regex & Guard, Schema Explorer, Field Mapper, Data Quality, Architecture, Export & Backup, Bulk Operations, Search Health, Dataset Intelligence, Search Environment, Performance, Anonymizer |
| **Billy** | AI assistant for KQL, dashboards, and architecture |
| **Help & Docs** | Documentation, keyboard shortcuts, about |
| **Settings** | Theme, connections, mobile layout, preferences |

---

## Features at a glance

| Area | Highlights |
|------|------------|
| **Charts** | **102** built-in visualizations (55 core + 47 gallery) + custom plugins |
| **Metrics** (via ⌘K — hidden from the sidebar for now) | PromQL-compatible Explorer, metric catalog/summary, monitors, active alerts, muting rules, notifications, presets, migration from PromQL/Datadog/Splunk, log-to-metrics extraction |
| **Converters** | Import dashboards from 9 vendors (Splunk XML/Studio, Sumo, Kibana/Elastic, Grafana, Datadog, New Relic, LogRhythm, Exabeam, CrowdStrike Falcon LogScale) plus Cribl JSON; convert queries from 12 languages |
| **Canvas** | Free-form layout with drawing tools, photo editing, video/audio, particles, symmetry |
| **Security** | 10 security visualizations (MITRE ATT&CK, kill chain, attack path, 3D globe, …), Compliance Mapper, Anomaly Narratives, Anonymizer / Cribl Guard scanning |
| **Automation** | Scheduled Reports, Bulk Operations, Export & Backup, Webhook Actions, Drill-Through Links |
| **Analytics** | Anomaly Detector, Forecaster, Data Quality, Data Journey, Field Lineage, Cost Optimizer, ROI Calculator, Capacity Planner, TCO Comparison |
| **Developer** | KQL REPL, Schema Explorer, API Explorer, Custom Functions, Plugin SDK, Field Mapper, Webhooks, Notebooks, KQL Formatter, Query Templates, Query Workbench |
| **Migration** | Splunk Migration Wizard (6-step), Side-by-Side Compare (SPL vs KQL), AI Dashboard Builder, Migration Readiness |
| **NOC & Executive** | Status Wall (real-time health grid), Executive Mode (auto-cycling slides), Mobile Layout (responsive reflow) |
| **AI Intelligence** | **✦ Insights** (Compose · Understand · Polish), Cribl Search Tools Assist (⌘/Ctrl-J), Billy NL→KQL, Query Cost Estimator |
| **Cross-Dashboard** | Global Search, Dashboard Diff, Drill-Through Links, Multi-Tenant Views, Dashboard Lifecycle |
| **Collaboration** | Real-time cursors (Yjs), version history, access control |
| **Theme** | Auto dark/light from Cribl host; manual override in standalone |

---

## Built-in visualizations (102)

55 core visualizations plus 47 gallery plugins.

### Basic (24)
Column, Horizontal Bar, Radial Bar, Line, Bump, Area, Pie, Donut, Scatter, Bubble, Single Value, Arc Gauge, Table, Events, KPI Strip, Radial/Marker/Speedometer/Liquid Fill/Linear Gauge, Honeycomb Status, App Status Tiles, Status Grid, Funnel

### Statistical & Time-Series (9)
Heatmap, Box Plot, Parallel Coordinates, Calendar Heatmap, Candlestick, Waterfall, Dumbbell, Bullet, Gantt

### Networks & Hierarchies (7)
Sankey, Network Graph, Chord, Flow (React Flow), Tree, Treemap, Sunburst

### Geo & 3D (5)
Isometric Bars, 3D Scatter, 3D Surface, 3D Network, Geo Choropleth

### Security (10)
MITRE ATT&CK Matrix, Cyber Kill Chain, Detection Coverage Radar, Process Lineage, Attack Path Graph, Auth Anomaly Heatmap, Geo Attack Flows, 3D Globe, Alert Correlation, IOC Velocity

### Gallery — ECharts (20)
Theme River, Pictorial Bar, Wind Rose, Polar Scatter, Liquid Fill Gauge, Nightingale Rose, Bar Race, Circular Graph, Sankey (Vertical), 3D Gauge/Funnel/Pie, Stacked Donut, Calendar Scatter, Radar (Polar), Bubble Map, River Flow, Polar Bar, 3D Globe/Scatter

### Gallery — D3 (17)
Word Cloud, Radial Tree, Force Bubbles, Streamgraph, Hexbin, Zoomable Sunburst, Violin, Beeswarm, Lollipop, Arc Diagram, Packed Circles, Ridgeline, Slope, Waffle, Dot Plot, Histogram, Marimekko

### Gallery — Chart.js (10)
Radar, Polar Area, Bubble, Mixed Bar + Line, Stacked Bar, Scatter, Nested Doughnut, Stacked Area, Floating Bar, Timeline

---

## Plugins

Open **+ Plugins** on Search to install from the gallery or paste a trusted ESM URL. Plugin code runs with full page permissions.

---

## Tools & Automation (80+)

Cribl Search Tools includes a full productivity suite accessible from the sidebar or via ⌘K:

- **Query tools:** KQL playground, REPL notebook, Query Studio (library, explainer, translator), regex lab, custom macro functions, field mapping, schema exploration
- **Security & compliance:** security visualizations, Compliance Mapper, Anomaly Narratives (AI incident summaries), Anonymizer with Cribl Guard scanning
- **Automation:** scheduled report generation, bulk operations, export & backup, webhook integrations, drill-through links
- **Collaboration:** dashboard notes & comments, annotations, Present mode, shareable snapshots
- **Analytics:** anomaly detection, metric forecasting, capacity planning, cost optimization, SLA monitoring, TCO and ROI calculators
- **Migration:** guided Splunk migration wizard, side-by-side SPL/KQL comparison, dashboard and query converters, migration readiness
- **NOC & Executive:** Status Wall (real-time health grid), Executive Mode (auto-cycling lobby display), mobile/tablet responsive layouts
- **AI Intelligence:** **✦ Insights** (live KQL coaching, result Explain, Data Story, dashboard Tidy/Beautify), Billy natural language → KQL, Query Cost Estimator (pre-run cost analysis), **✦ Assist** (⌘/Ctrl-J) for deep expert review
- **Cross-Dashboard:** Global Search, Dashboard Diff (version comparison), Drill-Through Links, Multi-Tenant Views (MSSP isolation), Embedded Notebooks, Dashboard Lifecycle

---

## Need developer docs?

Full source documentation (architecture, tests, parity, converters) is in the source repo README.md and docs/.

---

## License

Licensed under the **Apache License, Version 2.0**. See [LICENSE](../LICENSE).
