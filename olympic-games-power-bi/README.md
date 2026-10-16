# Olympic Games Data Analysis | Power BI

An interactive Power BI project exploring Olympic Games history, athlete participation, country performance, medals, sports, events, and host-nation performance.

> **Project status:** In progress. This repository contains the Power BI report supplied for the project and a project guide. Any numerical findings should be verified against the report and source data before being presented as conclusions.

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

These are analysis questions, not findings. Confirm results from the actual data before reporting rankings, percentages, or trends.

## Important metric definitions

- **Athlete medal records** are not necessarily the same as **medals awarded**. Team events can create multiple athlete records for one awarded medal.
- **Events held** in an edition are different from **events added** for the first time.
- Use a stable event identifier across editions where possible. If using sport + event title, standardize names and check that the combination uniquely identifies an event.
- If Summer and Winter editions are both present, use an edition identifier as well as year; two editions can occur in the same calendar year.
- Validate historical country/NOC codes and any changes in country naming.

## Open the report

1. Download and install [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Open `olympic-games-analysis.pbix`.
3. If Power BI requests a source-data path or credentials, follow the prompt and update the source settings as needed.
4. Review **Model view** and **Data view** to validate relationships and data quality.
5. Refresh the report only when the required source files are available.

## Publish this project to GitHub

1. Create a new repository on GitHub named `olympic-games-power-bi`.
2. Choose **Public** if you want to showcase it in your portfolio, or **Private** if the report/data should not be shared.
3. Upload the files in this folder, or use Git commands:

   ```bash
   git init
   git add README.md .gitignore assets olympic-games-analysis.pbix
   git commit -m "Add Olympic Games Power BI analysis"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/olympic-games-power-bi.git
   git push -u origin main
   ```

4. Replace `YOUR-USERNAME` with your GitHub username.

### File-size note

GitHub blocks ordinary Git files larger than 100 MB. If the PBIX is over that limit, use Git LFS or share the PBIX through a suitable file-hosting link and document it in this README. Before making the repository public, confirm you have permission to publish the report and any underlying data.

## Portfolio improvements

- Add screenshots of the finished report pages to `assets/`.
- Document the data source and cleaning steps.
- Add a data dictionary and explain important DAX measures.
- Include a short section with verified insights, each supported by a chart or measure.
- Remove private credentials, personal paths, and confidential data before publishing.
