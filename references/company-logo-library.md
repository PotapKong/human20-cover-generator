# Company Logo Library

Use this file when a Human 2.0 cover needs a recognizable third-party company, tool, platform, or product logo.

## Source

The local lookup workflow is adapted from the `logo-company` skill in `qwwiwi/codex-gpt-image-2-subscription`. It queries `glincker/thesvg`, an MIT-licensed public SVG library with thousands of brand icons.

The Human 2.0 skill does not bundle the full SVG database. It downloads only the requested logo into:

`_cache/company-logos/`

The cache is local and ignored by git.

## Find A Logo

Run from the skill folder or with an absolute path:

```powershell
.\scripts\find-company-logo.ps1 <brand-name> [default|mono|color|dark|light]
```

Examples:

```powershell
.\scripts\find-company-logo.ps1 openai default
.\scripts\find-company-logo.ps1 claude mono
.\scripts\find-company-logo.ps1 github default
```

The script prints the absolute SVG path on success and exits non-zero on failure.

## Variant Choice

- `default`: official full-color logo. Use when recognition matters and the mark sits on a neutral Human 2.0 surface.
- `mono`: single-color variant, often `currentColor`. Use when the logo must obey the Human 2.0 palette.
- `color`, `dark`, `light`: use only when the brand ships that variant and the cover background requires it.

If the requested variant is missing, the script falls back to `default`.

## Cover Workflow

1. Read `references/product-assets.md`.
2. Try `scripts/find-company-logo.ps1 <brand> default` or `mono` before web searching.
3. If the SVG is found, use it as an official asset for reference or final compositing.
4. If no SVG is found, search the official website, docs, GitHub org/repo, or brand page.
5. If no reliable asset is found, use a text-only product card. Do not invent the logo.

## Frequent Slugs

| Brand | Query / slug | Notes |
|---|---|---|
| OpenAI | `openai` | Use for parent company mark. |
| ChatGPT | `chatgpt`, `openai-chatgpt` | Prefer product-specific mark when the post is about ChatGPT. |
| Codex | `codex`, `codex-openai` | Use only when the logo exists in the cache source. |
| Claude | `claude` | Product mark. |
| Claude Code | `claude-code` | Coding-agent product mark. |
| Anthropic | `anthropic` | Company mark. |
| Gemini | `gemini`, `google-gemini` | Prefer Google Gemini product mark. |
| Grok | `grok`, `xai-grok` | xAI product mark. |
| Mistral | `mistral`, `mistral-ai` | Company/product mark. |
| Perplexity | `perplexity`, `perplexity-ai` | Product mark. |
| Midjourney | `midjourney` | Product mark. |
| Cursor | `cursor` | Coding tool. |
| GitHub | `github` | Platform mark. |
| GitHub Copilot | `github-copilot`, `copilot` | Product mark. |
| MCP | `mcp-model-context-protocol` | Protocol mark when available. |
| Hermes Agent | `hermes`, `hermes-agent`, `nousresearch-hermes` | Still verify with official Nous Research sources if exact fidelity matters. |
| Telegram | `telegram` | Social/platform mark. |
| Instagram | `instagram` | Social/platform mark. |
| YouTube | `youtube` | Social/platform mark. |
| TikTok | `tiktok` | Social/platform mark. |
| X / Twitter | `x-formerly-twitter`, `twitter` | Choose the brand named in the article. |
| Notion | `notion` | Product mark. |
| Supabase | `supabase` | Stack mark. |
| Vercel | `vercel` | Stack/company mark. |
| v0 | `v0`, `v0-vercel` | Product mark. |
| Figma | `figma` | Tool mark. |
| Linear | `linear` | Tool mark. |
| Docker | `docker` | Stack mark. |

## Quality Rules

- Prefer official SVGs over AI-redrawn marks.
- Keep third-party logos small-to-medium inside Human 2.0 layouts.
- Preserve aspect ratio.
- Do not recolor full-color brand marks unless the brand explicitly provides a mono/currentColor variant.
- Use `mono` for stylistic chips and `default` for recognition.
- Respect the brand's usage guidelines for public publishing.
