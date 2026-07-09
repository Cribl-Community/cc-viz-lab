# Viz Lab — what it does

**Viz Lab** is a **Cribl Search** app. Run **KQL**, browse **Events** and **Fields**, pick a **Chart**, and build **Dashboards** — in grid or free-form **Canvas** layout. Everything is one or two clicks from the sidebar.

---

## Quick use

1. **Search** — Write KQL (or plain English), set the time range, click Search.
2. Switch between **Events** (rows), **Fields** (column stats), or **Chart** (pick any visualization).
3. **Save** your search or drop it into a **Dashboard** panel.
4. **Dashboards** — Grid or Canvas layout, variables, imports, collaboration.

Press **⌘K** (Ctrl+K) anytime to jump to any page, dashboard, saved search, or action.

---

## Sidebar (flat — no scrolling)

The sidebar shows 8 primary items. Everything else lives under **More** or is reachable via ⌘K.

| Item | What you get |
|------|--------------|
| **Search** | KQL editor, time picker, Plain English, Events/Fields/Chart, streaming, annotations |
| **History** | Re-run or fork any previous search |
| **Saved** | Manage saved searches and collections; import/convert from Splunk and others |
| **Dashboards** | List, create, import, templates, export, health check, collections |
| **Query Studio** | Library + Explain + Format + Translate (7 languages) + Diff — all in one tabbed view |
| **Knowledge** | Lookups, parsers, regexes, grok, macros, lookup manager |
| **Investigate** | Timeline, Hunt Board (PEAK), IOC Lookup, Anonymizer, Run Book |
| **Wiz Viz** | AI assistant for KQL, dashboards, threat hunting, architecture |
| **More →** | Reports, Playbooks, Bulk Operations, Export Studio, Migration Wizard, ROI Calculator, Status Wall, Executive Mode, Notebooks, Demos, Settings, Help, and 50+ more tools |

---

## Features at a glance

| Area | Highlights |
|------|------------|
| **Charts** | **104** built-in visualizations (55 core + 49 gallery) + custom plugins |
| **Converters** | Import dashboards from 5 sources (Splunk XML/Studio, Sumo, Kibana, Grafana); translate queries from 7 languages |
| **Canvas** | Free-form layout with drawing tools, photo editing, video/audio, particles, symmetry |
| **Security** | Attack Simulator, Correlation Engine, Alert Builder, Auto-Investigate, Incident War Room, Attack Cinema (3D globe), PII Scanner, Compliance Mapper |
| **Automation** | Playbooks, Scheduled Reports, Bulk Operations, Webhook Actions, Smart Alerts from Panels |
| **Analytics** | Anomaly Detector, Metric Forecaster, Capacity Planner, Cost Optimizer, ROI Calculator, SLA Monitor, Data Quality |
| **Developer** | KQL Playground, KQL REPL, Regex Lab, Custom Functions, Plugin SDK, API Explorer, Data Lineage |
| **Migration** | Splunk Migration Wizard (6-step), Side-by-Side Compare (SPL vs KQL), NL Dashboard Generator |
| **Cinema** | Time Player, Cinema Mode, Attack Cinema, Presentation Mode, Dashboard Annotations |
| **NOC & Executive** | Status Wall (real-time health grid), Executive Mode (auto-cycling slides), Mobile Layout (responsive reflow) |
| **AI Intelligence** | Panel Explain, Anomaly Narratives, Query Cost Estimator, Wiz Viz chat, Copilot NL→KQL |
| **Cross-Dashboard** | Global Search, Dashboard Diff, Drill-Through Links, Multi-Tenant Views, Embedded Notebooks |
| **Collaboration** | Real-time cursors (Yjs), version history, access control |
| **Theme** | Auto dark/light from Cribl host; manual override in standalone |

---

## Built-in visualizations (104)

### Basic (24)
Column, Bar, Radial Bar, Line, Bump, Area, Pie, Donut, Scatter, Bubble, Single Value, Arc Gauge, Table, Events, KPI Strip, Radial/Marker/Speedometer/Liquid/Linear Gauge, Honeycomb, Status Tiles, Status Grid, Funnel

### Statistical & Time-Series (9)
Heatmap, Box Plot, Parallel Coordinates, Calendar Heatmap, Candlestick, Waterfall, Dumbbell, Bullet, Gantt

### Networks & Hierarchies (7)
Sankey, Network Graph, Chord, Flow (React Flow), Tree, Treemap, Sunburst

### Geo & 3D (8)
Isometric Bars, 3D Scatter, 3D Surface, 3D Network, Geo Choropleth, Globe (Three.js)

### Security (9)
MITRE ATT&CK Matrix, Kill Chain Funnel, Detection Radar, Process Tree, Attack Graph, Auth Heatmap, Geo Attack Flows, Alert Correlation, IOC Streamgraph

### Gallery — ECharts (22)
Theme River, Pictorial Bar, Wind Rose, Polar Scatter, Liquid Fill, Nightingale Rose, Bar Race, Circular Graph, Sankey Vertical, 3D Gauge/Funnel/Pie, Stacked Donut, Calendar Scatter, Radar Polar, Bubble Map, River Flow, Polar Bar, 3D Globe/Scatter

### Gallery — D3 (17)
Force Bubbles, Hexbin, Radial Tree, Streamgraph, Word Cloud, Zoomable Sunburst, Violin, Beeswarm, Lollipop, Arc Diagram, Packed Circles, Ridgeline, Slope, Waffle, Dot Plot, Histogram, Marimekko

### Gallery — Chart.js (10)
Bubble, Mixed, Polar Area, Radar, Scatter, Stacked Bar, Nested Doughnut, Stacked Area, Floating Bar, Timeline

---

## Plugins

Open **+ Plugins** on Search to install from the gallery or paste a trusted ESM URL. Plugin code runs with full page permissions.

---

## Tools & Automation (77+)

Viz Lab includes a full productivity suite accessible from the sidebar or via ⌘K:

- **Security:** Attack simulation, correlation rules, alert authoring, automated investigation, incident war rooms, PII scanning
- **Query tools:** KQL playground, REPL notebook, regex lab, custom macro functions, field mapping, schema exploration
- **Automation:** If/then playbooks, scheduled report generation, bulk operations, webhook integrations
- **Collaboration:** Panel comment threads, dashboard annotations, presentation mode, shareable snapshots, export studio
- **Analytics:** Anomaly detection, metric forecasting, capacity planning, cost optimization, SLA monitoring
- **Migration:** Guided Splunk migration wizard, side-by-side SPL/KQL comparison, ROI calculator
- **Cinema:** Animated time-based data playback, full-screen cinema mode, WarGames-style attack globe
- **NOC & Executive:** Status Wall (real-time health grid), Executive Mode (auto-cycling lobby display), Mobile/Tablet responsive layouts
- **AI Intelligence:** Panel Explain ("why did this spike?"), Anomaly Narratives (AI incident summaries), Query Cost Estimator (pre-run cost analysis)
- **Cross-Dashboard:** Global Search, Dashboard Diff (version comparison), Drill-Through Links, Multi-Tenant Views (MSSP isolation), Embedded Notebooks, Investigation Templates

---

## Need developer docs?

Full source documentation (architecture, tests, parity, converters) is in the source repo README.md and docs/.

---

## License

Licensed under the **Apache License, Version 2.0**. See [LICENSE](../LICENSE).
