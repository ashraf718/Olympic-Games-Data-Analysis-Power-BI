# Olympic-Games-Data-Analysis-Power-BI
An interactive Power BI project exploring Olympic Games history, athlete participation, country performance, medals, sports, events, and host-nation performance.

*Project status:** In progress. This repository contains the Power BI report supplied for the project and a project guide. Any numerical findings should be verified against the report and source data before being presented as conclusions.

## Project goals

- Explore medal performance by country and Olympic edition.
- Track participation and event-programme changes over time.
- Compare gold, silver, bronze, and total medal performance.
- Investigate athlete participation and medal-winning performance.
- Explore sports and events across Olympic editions.
- Examine whether host nations perform differently at home.

## File structure

```text
olympic-games-power-bi/
├── olympic-games-analysis.pbix
├── README.md
├── .gitignore
└── assets/
    └── dashboard-design-reference.png   # if included
```

## Power BI data model

The current model screenshot indicates tables such as:

- `Olympic Athlete Bio`
- `Olympic Athlete Event`
- `Olympic Results`
- `olympic games`
- `olympic country`
- `Olympic_Games_Medal ...`

Exact table names may vary in the PBIX file. Review relationships, cardinality, active relationships, and join keys in Model view before relying on measures.

## Suggested report pages

1. **Global Medal Overview** — KPI cards, top countries, medal trends, medal composition, events by year, and country map.
2. **Country Performance** — medal rankings, medal types, country trends, and medals by sport.
3. **Athlete Spotlight** — athlete rankings, medal winners, age patterns, and participation.
4. **Sports & Events** — event counts, medal distribution by sport, and programme growth.
5. **Host Nation Advantage** — host versus non-host results and performance around hosting editions.
6. **Participation & Historical Trends** — athletes, countries, and events across Olympic editions.

## Suggested questions to investigate

- Which countries have won the most medals?
- How has participation changed across Olympic editions?
- Which sports contribute the most medals for each country?
- Which events appear for the first time in each edition?
- How do host nations perform compared with their non-host editions?
- How do athlete medal outcomes vary by sport and gender?

## Important metric definitions

- **Athlete medal records** are not necessarily the same as **medals awarded**. Team events can create multiple athlete records for one awarded medal.
- **Events held** in an edition are different from **events added** for the first time.
- Use a stable event identifier across editions where possible. If using sport + event title, standardize names and check that the combination uniquely identifies an event.
- If Summer and Winter editions are both present, use an edition identifier as well as year; two editions can occur in the same calendar year.
- Validate historical country/NOC codes and any changes in country naming.
