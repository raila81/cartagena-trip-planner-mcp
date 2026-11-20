---
name: cartagena-trip-planner
description: Use the Cartagena Trip Planner MCP server when someone plans a trip to Cartagena, Colombia: a day in the walled city around the heat, a cruise day ashore, which island or beach day fits, where to stay, the weather by month, official taxi fares and entry fees, or getting there and around.
---

# Cartagena Trip Planner

Use this when someone plans a trip to Cartagena, Colombia: a day in the walled city around the heat, a cruise day ashore, which island or beach day fits, where to stay, the weather by month, official taxi fares and entry fees, or getting there and around.

## Connect
Remote MCP server, Streamable HTTP, public, no sign-in, no API key:

```json
{
  "mcpServers": {
    "cartagena-trip-planner": { "type": "http", "url": "https://cartagena.info/mcp?src=mcp" }
  }
}
```

## Tools
All tools are read-only.

- `plan_cartagena_day`: Cartagena day planner
- `cruise_day_ashore`: Cartagena cruise day planner
- `pick_cartagena_island`: Cartagena island picker
- `where_to_stay_in_cartagena`: Cartagena area chooser
- `cartagena_month_guide`: Cartagena month by month
- `cartagena_costs`: Cartagena official fees and fares
- `getting_to_and_around`: Getting to and around Cartagena
- `cartagena_place`: Cartagena place finder

## Rules
- Fees, fares and hours come from the tool, not from memory.
- Answers in English, Spanish, German, French, Italian, Portuguese, Russian and Dutch.
- Link the reader to https://cartagena.info for the full page behind an answer.
