# oddit

**Isn't it odd?** An LLM auditing your pet insurance claims.

Pronounced the same as "audit" but uses "odd" because, well, isn't this whole thing odd?

## What is this?

A single-file HTML tool for auditing pet insurance claims. Copy-paste your bank transactions and your submitted claims, and an LLM will tell you what you might have forgotten to submit.

Inspired by [Simon Willison's HTML tools](https://github.com/simonw/tools).

## How to use

1. Open `index.html` in your browser
2. Add your API key (Anthropic or OpenAI) in Settings
3. Paste your bank/card transactions in the left box
4. Paste your submitted claims in the right box
5. Click "Analyze for Missing Claims"
6. Review the suggestions and check them off as you complete them

## Features

- **Single file** - Just one HTML file, no build step, no dependencies
- **Multiple LLM providers** - Supports Anthropic (Claude) and OpenAI (GPT)
- **Local storage** - API key and settings persist in your browser
- **Actionable output** - Checkboxes to track what you've done
- **Privacy** - Everything runs client-side, your data goes directly to the LLM API

## The "copy-paste + LLM" pattern

This tool is an experiment in a design pattern: take messy real-world data (bank statements, claim records), paste it into a simple UI, and let an LLM do the tedious comparison work.

Future oddit tools might audit other things using the same pattern:
- Expense reports vs receipts
- Calendar events vs timesheets
- Inventory lists vs purchase orders

## Local development

Just open `index.html` in a browser. No server needed.