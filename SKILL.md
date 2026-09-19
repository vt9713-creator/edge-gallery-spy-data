---
name: SPY Market Data
description: Retrieves read-only daily market data for SPY.
---

# SPY Market Data

Use this skill when the user asks for current or recent SPY market data.

This skill is read-only.

Call the `run_js` tool with:
- script name: index.html
- data: A JSON string containing:
  - symbol: String. The stock symbol to retrieve.

For this first test, use:
- symbol: "SPY"

The JavaScript skill retrieves the latest available daily candle.

Return the values exactly as provided by the data source.

Return:
- timestamp
- open
- high
- low
- close
- volume

If the data source fails or returns incomplete data, report the error.

Never invent, estimate, or substitute a market price.

Do not:
- place trades
- connect to a brokerage account
- request brokerage credentials
- modify trading strategies
- modify files outside this skill
