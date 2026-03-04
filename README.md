![Comming soon](https://img.shields.io/badge/Comming%20soon-F2B84B?style=for-the-badge&labelColor=F7DE9E)

# Norwegian Statistics Agent — Support & Docs

This repository provides user-facing information, support, and policies for the "Norwegian Statistics Agent" published for Microsoft Teams and Microsoft 365 Copilot Chat.

The agent helps you discover and import tabular data from Statistics Norway (SSB) via PX-Web HTTP queries, so you can analyze the results directly in Copilot.

> [!IMPORTANT]
> Data from Statistics Norway ([SSB](https://www.ssb.no/)), retrieved via the open [StatBank API](https://www.ssb.no/en/api). Licensed under Creative Commons Attribution 4.0 ([CC BY 4.0]()). The data has been processed by this application.

## Overview

- Runs in Microsoft Teams and Microsoft 365 Copilot Chat (may require Copilot licenses such as pay-as-you-go or Microsoft 365 Copilot add-in).
- Language: English.
- Capabilities:
  - Search SSB tables by topic/keywords and return matching table IDs with short descriptions.
  - Retrieve parameters and available values for a selected table.
  - Import table data by specifying filters for parameters; if a parameter is omitted, the agent uses `*` (all values) for that parameter.
  - Presents imported data as an HTML table in the chat.

## Important limitations

- Some tables are too large to download completely due to data size limits and platform constraints.
- The SSB API and Copilot may enforce rate limits or practical limits on result size.
- Availability, functionality, and maintenance are not guaranteed.

## Quick start

1. Open a Microsoft 365 Copilot Chat and mention the agent (e.g., `@Norwegian Statistics Agent`).
2. Ask the agent to search tables by topic/keywords; it will reply with table IDs and descriptions.
3. Ask for parameters of a specific table ID to see available fields and values.
4. Request an import from that table, specifying parameter filters as needed. Unspecified parameters default to `*` (all).
5. The agent returns an HTML table with the requested data.
6. Switch off the agent (click the X next to the agent) and continue analysis using core Copilot features (e.g., create dataframes, use Python for charts, analyze, export, or collaborate with other agents).

## APIs and data sources

- Uses Statistics Norway PX-Web HTTP queries.
- Not all tables can be downloaded in full; prefer focused filters.
- Users must comply with the Statistics Norway API terms and any applicable usage restrictions.

## Example

- See the example analysis in the [Report](Report/) folder for a sample diagram, analysis, and forecast exported from a chat session.

## Sample Screenshots

Below are sample screenshots illustrating the agent workflow.

![Search by topic](./Images/2%20Search%20by%20topic.png)

Diagrams can be obtained using the Microsoft 365 Copilot Chat.

![Salmon Export Chart](./Images/8%20salmon_export_chart_labeled.png)

For more details, see [HOW_IT_WORKS.md](HOW_IT_WORKS.md) Issues in this repository. See [SUPPORT.md](SUPPORT.md).

## Privacy

- The agent does not collect personal data. See [PRIVACY.md](PRIVACY.md).

## Terms of Use

- Free, AS-IS, with no warranty or SLA; availability is not guaranteed. See [TERMS OF USE.md](TERMS%20OF%20USE.md).
