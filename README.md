# Botswana Land Plots & Gaborone Lot Lookup MCP

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Botswana land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- ~865k plots nationwide from the LAPCAS land administration project, each with its plot number and, on about a third, the village or town
- The City of Gaborone's ~52k lots, with survey record, approved survey diagram and township extension
- Plot lookup by number and village (`plot 6121 Ghanzi`), Gaborone lot number (`35571`, `2881-KO`), or coordinates
- Satellite and street map images of a plot and its neighbours, labelled by plot number

Plots have no owner, tenure (tribal, state or freehold) or price information.

## Connect

```
https://bumiatlas.com/mcp/botswana
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/botswana](https://bumiatlas.com/mcp-docs/botswana).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `BW_plot_search` | Find plots by number and village, Gaborone lots by lot number, or both by `latitude, longitude`; each result is the whole record, the boundary as GeoJSON on request |
| `BW_plot_image` | Satellite or street map image of a plot or point, with every plot in view outlined and labelled with its plot number |

## Example prompts

- *"Which plot is at -24.6282, 25.9231?"*
- *"Find plot 6121 in Ghanzi and show it on satellite imagery."*
- *"Look up Gaborone lot 35571: what's its survey record and diagram number?"*
- *"How large is this plot?"*

## Data source

Plots © Department of Lands, Botswana (LAPCAS), via Botswana Fibre Networks' public GIS. A copy of public data for research, not a legal land record.
