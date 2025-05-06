# 🤘 Welcome to Stagehand Next.js Deploy with Replit!

Hey! This is a Next.js project built with [Stagehand](https://github.com/browserbase/stagehand).

You can build your own web agent using: `npx create-browser-app`!

## Setting the Stage

Stagehand is an SDK for automating browsers. It's built on top of [Playwright](https://playwright.dev/) and provides a higher-level API for better debugging and AI fail-safes.

## Curtain Call

Get ready for a show-stopping development experience. Just run:

```bash
npm install && npm run dev
```

## What's Next?

### Add your API keys

This project defaults to using OpenAI, so it's going to throw a fit if you don't have an OpenAI API key.

To use Anthropic (or other LLMs), you'll need to edit [stagehand.config.ts](stagehand.config.ts) to use the appropriate API key.

Required API keys/environment variables are in the `.env.example` file. 
You have to enter these into the Secrets Pane. Docs on how to use that [here](https://docs.replit.com/replit-workspace/workspace-features/secrets).

To run on Browserbase, add your API keys to .env and change `env: "LOCAL"` to `env: "BROWSERBASE"` in [stagehand.config.ts](stagehand.config.ts).

### Use Anthropic Claude 3.5 Sonnet

1. Add your API key to .env
2. Change `modelName: "gpt-4o"` to `modelName: "claude-3-5-sonnet-latest"` in [stagehand.config.ts](stagehand.config.ts)
3. Change `modelClientOptions: { apiKey: process.env.OPENAI_API_KEY }` to `modelClientOptions: { apiKey: process.env.ANTHROPIC_API_KEY }` in [stagehand.config.ts](stagehand.config.ts)
