# SDK Tutorials

Simple Node.js examples showing how to call three popular AI model SDKs:

| File | SDK | What it does |
|------|-----|--------------|
| `openai-sdk.js` | [OpenAI](https://github.com/openai/openai-node) | Sends a basic prompt using the Responses API |
| `structure-sdk.js` | OpenAI + [Zod](https://zod.dev) | Extracts **structured JSON output** (calendar event) from text |
| `claude-sdk.js` | [Anthropic](https://github.com/anthropics/anthropic-sdk-typescript) | Sends a message to Claude |
| `gemini-sdk.js` | [Google GenAI](https://github.com/googleapis/js-genai) | Asks Gemini a question |

## Setup

1. Install dependencies:

   ```bash
   npm install
   ```

2. Copy `.env.example` to `.env` and add your API keys:

   ```env
   OPENAI_API_KEY=your_openai_api_key
   ANTHROPIC_API_KEY=your_anthropic_api_key
   GEMINI_API_KEY=your_gemini_api_key
   ```

## Run

```bash
npm run openai       # OpenAI basic prompt
npm run structured   # OpenAI structured output with Zod
npm run claude       # Anthropic Claude
npm run gemini       # Google Gemini
```

Or run any file directly, e.g. `node claude-sdk.js`.

## Notes

- Requires Node.js 18+ (uses ES modules and top-level `await`).
- `.env` is git-ignored — never commit your API keys.
