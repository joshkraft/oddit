# oddit

**Isn't it odd?** LLM-powered audit tools.

Pronounced the same as "audit" but uses "odd" because, well, isn't this whole thing odd?

## What is this?

A collection of single-file HTML tools that use LLMs as an audit layer. Copy-paste messy real-world data, let an LLM do the tedious comparison work, get actionable checklists.

Inspired by [Simon Willison's HTML tools](https://github.com/simonw/tools).

## Tools

### Pet Insurance Auditor (`tools/pet-insurance.html`)
Compare bank transactions against submitted pet insurance claims. Find expenses you forgot to file.

### Subscription Auditor (`tools/subscriptions.html`)
Find forgotten subscriptions hiding in your bank statements. See your true monthly/annual subscription costs and identify charges you might want to cancel.

## How to use

1. Open `index.html` to see available tools, or go directly to a tool
2. Add your API key (Anthropic, OpenAI, or Google) in Settings
3. Paste your data in the input boxes
4. Click Analyze
5. Mark items as done or irrelevant as you work through them

## Features

- **Single file tools** - No build step, no dependencies
- **Multiple LLM providers** - Anthropic (Claude), OpenAI (GPT), Google (Gemini)
- **Local storage** - API key and settings persist in your browser
- **Actionable output** - Mark items done or irrelevant
- **Privacy** - Everything runs client-side, your data goes directly to the LLM API

## The "copy-paste + LLM" pattern

Each tool follows the same pattern: paste in messy real-world data, let an LLM analyze and compare, get back a checklist of things to do.

Future tools might audit:
- Expense reports vs receipts
- Calendar events vs timesheets
- Inventory lists vs purchase orders

## Local development

Just open `index.html` in a browser. No server needed.