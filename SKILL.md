---
name: SPY Market Data
description: Retrieves read-only daily market data for SPY and returns timestamp, open, high, low, close, and volume.
---

# SPY Market Data

Use this skill only when the user asks for SPY market data.

This skill is read-only.

It must not:
- place trades
- connect to a brokerage account
- request brokerage credentials
- modify trading strategies
- modify files outside this skill

When retrieving data, return the values exactly as provided by the data source.

If the data source fails or returns incomplete data, report the error. Never invent, estimate, or substitute a market price.

For each daily candle, return:

- timestamp
- open
- high
- low
- close
- volume

The first version of this skill should retrieve only the latest available daily SPY candle.
