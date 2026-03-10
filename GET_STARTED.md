# Get started

This document explains how the Norwegian Statistics Agent operates within Microsoft Teams and Microsoft 365 Copilot Chat to help you locate and import tables from Statistics Norway (SSB).

For suggestions about prompts, explore the Prompt Gallery.

## Interaction flow

- Choose the agent on Teams or on Microsoft 365 Copilot Chat.
- Ask to search tables by topic/keywords. The agent queries SSB PX-Web endpoints and returns matching table IDs with short descriptions.
- Request parameters for a specific table ID to discover available fields and values.
- Ask the agent to import data from that table, providing filters for parameters.
  - If a parameter is not provided, the agent uses `*` (all values) for that parameter.
- The agent returns data formatted as an HTML table in the chat.
- Ask to draw charts with the data.
- Choose the agent on Teams or on Microsoft 365 Copilot.
- Ask to search tables by topic/keywords. The agent queries SSB PX-Web endpoints and returns matching table IDs with short descriptions.
- Request parameters for a specific table ID to discover available fields and values.
- Ask the agent to import data from that table, providing filters for parameters.
  - If a parameter is not provided, the agent uses `*` (all values) for that parameter.
- The agent returns data formatted as an HTML table in the chat.
- Ask the agent to draw charts with the data.
- Ask the agent to analyze the data.
- Ask to export the data in several file formats: CSV, JSON, TXT, DOCX, PPTX, PDF.

## Limits and constraints

- Some SSB tables are too large to download in full due to size and platform constraints.
- The SSB API and Copilot may impose rate limits or practical limits on response sizes.
- Availability, functionality, and maintenance of the agent are not guaranteed; this is a free test offering.
- Some SSB tables are too large to download in full due to size and platform constraints.
- The SSB API and Copilot may impose rate limits or practical limits on response sizes.
- Agents should aim to respond within nine seconds in Copilot; long-running imports may be limited and should display progress or warnings.
- Availability, functionality, and maintenance of the agent are not guaranteed; this is a free test offering.

## Example output

- See [Report](Report) for a sample analysis exported from a chat, including diagrams, analysis, and forecast.

## Sample Screenshots

Below are screenshots:

<figure>
  <img src="./Images/01 Teams Mobile H.jpg" alt="Teams Mobile - Import data" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Mobile</strong> — Import data.</figcaption>
</figure>

<figure>
  <img src="./Images/02 Teams Mobile H.jpg" alt="Teams Mobile - Draw a chart" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Mobile</strong> — Draw a chart.</figcaption>
</figure>

<figure>
  <img src="./Images/03 Teams Desktop.png" alt="Teams Desktop - Import data" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Desktop</strong> — Import data.</figcaption>
</figure>

<figure>
  <img src="./Images/04 Teams Desktop.png" alt="Teams Desktop - Draw a chart" style="width:50%;height:auto;" />
  <figcaption><strong>Teams Desktop</strong> — Draw a chart.</figcaption>
</figure>

<figure>
  <img src="./Images/05 Microsoft 365 Copilot.png" alt="Microsoft 365 Copilot - Import data" style="width:50%;height:auto;" />
  <figcaption><strong>Microsoft 365 Copilot</strong> — Import data.</figcaption>
</figure>
