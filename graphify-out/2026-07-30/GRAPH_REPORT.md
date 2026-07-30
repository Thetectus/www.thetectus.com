# Graph Report - .  (2026-07-15)

## Corpus Check
- Corpus is ~11,565 words - fits in a single context window. You may not need a graph.

## Summary
- 45 nodes · 55 edges · 8 communities
- Extraction: 73% EXTRACTED · 27% INFERRED · 0% AMBIGUOUS · INFERRED: 15 edges (avg confidence: 0.82)
- Token cost: 228,896 input · 0 output

## Community Hubs (Navigation)
- Homepage Brand Story
- Portfolio Product Family
- Service Offerings
- Social Share Image
- Favicon SVG Mark
- Favicon 32px Mark
- Apple Touch Icon
- Favicon 16px Mark

## God Nodes (most connected - your core abstractions)
1. `The Tectus Homepage` - 8 edges
2. `Portfolio Page` - 8 edges
3. `Services Section` - 7 edges
4. `FieldTrack Product (Portfolio featured card)` - 7 edges
5. `FieldTrack Product (Homepage description)` - 4 edges
6. `Tectus Open Graph Preview Image` - 4 edges
7. `Tectus (software house, Angola)` - 4 edges
8. `404 Not Found Page` - 3 edges
9. `Tectus Favicon (32x32)` - 3 edges
10. `Tectus Favicon Icon (favicon.svg)` - 3 edges

## Surprising Connections (you probably didn't know these)
- `Multi-language Selector (PT/EN/FR, Portfolio)` --semantically_similar_to--> `Multi-language Selector (PT/EN/FR, Homepage)`  [INFERRED] [semantically similar]
  portfolio.html → index.html
- `FieldTrack Product (Portfolio featured card)` --references--> `FieldTrack Product (Homepage description)`  [INFERRED]
  portfolio.html → index.html
- `404 Not Found Page` --references--> `Portfolio Page`  [EXTRACTED]
  404.html → portfolio.html
- `The Tectus Brand/Logo (404 page)` --references--> `The Tectus (Company)`  [INFERRED]
  404.html → index.html
- `Portfolio Page` --references--> `The Tectus Homepage`  [EXTRACTED]
  portfolio.html → index.html

## Hyperedges (group relationships)
- **Homepage Navigation Flow (Nav links to Hero/About/Services/Product sections)** — index_hero_section, index_about_section, index_services_section, index_product_section [EXTRACTED 1.00]
- **The Tectus SaaS Product Portfolio (FieldTrack, FleetTrack, AssetTrack, DocFlow)** — portfolio_fieldtrack, portfolio_fleettrack, portfolio_assettrack, portfolio_docflow [INFERRED 0.80]

## Communities (8 total, 0 thin omitted)

### Community 0 - "Homepage Brand Story"
Cohesion: 0.28
Nodes (9): 404 Not Found Page, The Tectus Brand/Logo (404 page), About Section (Quem Somos), FieldTrack Product (Homepage description), Hero Section, The Tectus Homepage, Product Section (FieldTrack), SaaS Products Service (+1 more)

### Community 1 - "Portfolio Product Family"
Cohesion: 0.33
Nodes (9): Multi-language Selector (PT/EN/FR, Homepage), AssetTrack Product (in development), DocFlow Product (in development), FieldTrack Product (Portfolio featured card), Project Filter Bar (All/Live/Dev/SaaS/Oil&Gas/Logistics), FleetTrack Product (in development), Multi-language Selector (PT/EN/FR, Portfolio), Portfolio Page (+1 more)

### Community 2 - "Service Offerings"
Cohesion: 0.33
Nodes (6): Custom Software Service, Dashboards & Reports Service, Integrations & APIs Service, Process Automation Service, Services Section, Support & Maintenance Service

### Community 3 - "Social Share Image"
Cohesion: 0.53
Nodes (6): thetectus.com (domain), Headline: 'Software que resolve problemas reais.', Tectus Open Graph Preview Image, Subheadline: 'Software house angolana — soluções sob medida e produtos SaaS próprios para África e além.', Tectus (software house, Angola), The Tectus (brand mark)

### Community 4 - "Favicon SVG Mark"
Cohesion: 0.50
Nodes (5): Blue Filled Circle Symbol, Darker Blue Ring Outline on Circle, Tectus Favicon Icon (favicon.svg), Dark Navy Rounded-Square Background, Tectus Website Brand

### Community 5 - "Favicon 32px Mark"
Cohesion: 0.67
Nodes (4): Blue Dot / Circle Symbol, Dark Rounded-Square Background, Tectus Favicon (32x32), Tectus Website Brand

### Community 6 - "Apple Touch Icon"
Cohesion: 0.67
Nodes (3): Apple Touch Icon (Tectus Brand Mark), Dark Navy Rounded-Square Background, Blue Dot Symbol

### Community 7 - "Favicon 16px Mark"
Cohesion: 1.00
Nodes (3): Tectus Favicon (16x16), Circular Dark Logomark with Light Dot Accent, Tectus Brand Identity

## Knowledge Gaps
- **12 isolated node(s):** `About Section (Quem Somos)`, `Custom Software Service`, `Process Automation Service`, `Dashboards & Reports Service`, `Integrations & APIs Service` (+7 more)
  These have ≤1 connection - possible missing edges or undocumented components.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `The Tectus Homepage` connect `Homepage Brand Story` to `Portfolio Product Family`, `Service Offerings`?**
  _High betweenness centrality (0.148) - this node is a cross-community bridge._
- **Why does `Services Section` connect `Service Offerings` to `Homepage Brand Story`?**
  _High betweenness centrality (0.113) - this node is a cross-community bridge._
- **Why does `Portfolio Page` connect `Portfolio Product Family` to `Homepage Brand Story`?**
  _High betweenness centrality (0.094) - this node is a cross-community bridge._
- **Are the 4 inferred relationships involving `FieldTrack Product (Portfolio featured card)` (e.g. with `AssetTrack Product (in development)` and `DocFlow Product (in development)`) actually correct?**
  _`FieldTrack Product (Portfolio featured card)` has 4 INFERRED edges - model-reasoned connections that need verification._
- **What connects `About Section (Quem Somos)`, `Custom Software Service`, `Process Automation Service` to the rest of the system?**
  _12 weakly-connected nodes found - possible documentation gaps or missing edges._