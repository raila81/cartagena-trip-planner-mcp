# Cartagena Trip Planner MCP server

Plans a trip to Cartagena de Indias on the Caribbean coast of Colombia. Give a month or a date and get a day in the walled city timed around the heat, with sunset on the city wall. Cruise passengers get what fits between arrival and all aboard. Also: which island or beach day fits (Baru and Playa Blanca, the Rosario Islands, Tierra Bomba, Cholon, San Bernardo), which neighbourhood to stay in, the month-by-month weather, official airport taxi fares and entry fees, getting there and around, and facts on the main sights. Answers in English, Spanish, German, French, Italian, Portuguese, Russian and Dutch.

Independent guide from cartagena.info, published by BRS Properties Co., Ltd. Not affiliated with the city of Cartagena, the national park or any tour seller.

- **Website:** [cartagena.info](https://cartagena.info)
- **Documentation:** [cartagena.info/ai-assistants/](https://cartagena.info/ai-assistants/)
- **Endpoint:** `https://cartagena.info/mcp` (MCP Streamable HTTP, public, no authentication, no API key)
- **MCP Registry:** `info.cartagena/cartagena-trip-planner`

## Tools

- `plan_cartagena_day`: Cartagena day planner (read-only)
- `cruise_day_ashore`: Cartagena cruise day planner (read-only)
- `pick_cartagena_island`: Cartagena island picker (read-only)
- `where_to_stay_in_cartagena`: Cartagena area chooser (read-only)
- `cartagena_month_guide`: Cartagena month by month (read-only)
- `cartagena_costs`: Cartagena official fees and fares (read-only)
- `getting_to_and_around`: Getting to and around Cartagena (read-only)
- `cartagena_place`: Cartagena place finder (read-only)

## Connect

```json
{
  "mcpServers": {
    "cartagena-trip-planner": {
      "type": "streamable-http",
      "url": "https://cartagena.info/mcp?src=mcp"
    }
  }
}
```

Claude: Settings → Connectors → Add custom connector → `https://cartagena.info/mcp?src=claude`.

## Example prompts

- "Plan a day in Cartagena, Colombia in March around the heat."
- "Our cruise ship docks in Cartagena at 8:00 in February and all aboard is 17:30. What can we fit in?"
- "We have one full day in January and want to swim, but we hate fast boats on a rough sea. Which island or beach?"
- "What is the official taxi fare from Cartagena airport to Getsemani?"
