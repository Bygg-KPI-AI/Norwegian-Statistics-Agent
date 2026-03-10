![Comming soon](https://img.shields.io/badge/Comming%20soon-F2B84B?style=for-the-badge&labelColor=F7DE9E)

# Norwegian Statistics Agent — Support & Docs

This repository provides user-facing information, support, and policies for the "Norwegian Statistics Agent" published for Microsoft Teams and Microsoft 365 Copilot Chat.

The agent helps you discover and import tabular data from Statistics Norway (SSB) via PX-Web HTTP queries, so you can analyze the results directly in Copilot.

> [!IMPORTANT]
> Data provided by Statistics Norway ([SSB](https://www.ssb.no/)) via the StatBank API ([StatBank API](https://www.ssb.no/en/api)). SSB data and content are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You must provide attribution to "Statistics Norway (SSB)" and include links to the license and SSB's license page ([SSB license page](https://www.ssb.no/diverse/lisens)).
>
> Note: Some materials (for example photographs) may have separate rights and are not covered by CC BY 4.0. Data containing personal or confidential information may not be covered by CC BY 4.0 — check the specific dataset's license and SSB notices before redistributing extracted data.

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

Below are sample screenshots illustrating the use of the agent:

<figure>
  <img src="./Images/Teams%20Mobile.png" alt="Teams Mobile" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Mobile</strong> — Mobile client view in Microsoft Teams.</figcaption>
</figure>

<figure>
  <img src="./Images/Teams%20Desktop.png" alt="Teams Desktop" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Desktop</strong> — Desktop client view in Microsoft Teams.</figcaption>
</figure>

<figure>
  <img src="./Images/Microsoft%20365%20Copilot.png" alt="Microsoft 365 Copilot" style="width:50%;height:auto;" />
  <figcaption><strong>Microsoft 365 Copilot</strong> — Agent interaction inside Microsoft 365 Copilot Chat.</figcaption>
</figure>

For more details, see [GET_STARTED.md](GET_STARTED.md) Issues in this repository. See [SUPPORT.md](SUPPORT.md).

## Privacy

- The agent does not collect personal data. See [PRIVACY.md](PRIVACY.md).

## Permissions

- See [PERMISSIONS.md](PERMISSIONS.md) for the permissions required by the app.

## Terms of Use

- Free, AS-IS, with no warranty or SLA; availability is not guaranteed. See [TERMS OF USE.md](TERMS_OF_USE.md).
