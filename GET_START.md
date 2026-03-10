# Get start

This document explains how the Norwegian Statistics Agent operates within Microsoft Teams and Microsoft 365 Copilot Chat to help you locate and import tables from Statistics Norway (SSB).

For suggestions about promts, explore the Prompt Gallery.

## Interaction flow

- Choose the agent on Teams or on Microsoft 365 Copilot.
- Ask to search tables by topic/keywords. The agent queries SSB PX-Web endpoints and returns matching table IDs with short descriptions.
- Request parameters for a specific table ID to discover available fields and values.
- Ask the agent to import data from that table, providing filters for parameters.
  - If a parameter is not provided, the agent uses `*` (all values) for that parameter.
- The agent returns data formatted as an HTML table in the chat.
- Ask to draw charts with the data.
- Ask to make analysis with the data.
- Ask to export the data in several file formats: *.csv, *.json, *.txt, *.docx

## Limits and constraints

- Some SSB tables are too large to download in full due to size and platform constraints.
- The SSB API and Copilot may impose rate limits or practical limits on response sizes.
- Availability, functionality, and maintenance of the agent are not guaranteed; this is a free test offering.

## Example output

- See [Report](Report) for a sample analysis exported from a chat, including diagrams, analysis, and forecast.

## Sample Screenshots

Below are screenshots:

<figure>
  <img src="./Images/01%20Teams%20Mobile%20H.jpg" alt="01 Teams Mobile H" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Mobile - 'Import data'</strong></figcaption>
</figure>

<figure>
  <img src="./Images/02%20Teams%20Mobile%20H.jpg" alt="02 Teams Mobile H" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Mobile - 'Draw a chart'</strong></figcaption>
</figure>

<figure>
  <img src="./Images/03%20Teams%20Desktop.png" alt="03 Teams Desktop" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Desktop - 'Import data'</strong></figcaption>
</figure>

<figure>
  <img src="./Images/04%20Teams%20Desktop.png" alt="04 Teams Desktop" style="width:50%;height:auto;" />
  <figcaption><strong>04 Teams Desktop - 'Draw a chart'</strong></figcaption>
</figure>

<figure>
  <img src="./Images/05%20Microsoft%20365%20Copitlot.png" alt="05 Microsoft 365 Copitlot" style="width:50%;height:auto;" />
  <figcaption><strong>05 Microsoft 365 Copitlot - 'Import data'</strong></figcaption>
</figure>
