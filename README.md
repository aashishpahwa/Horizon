<div align="center">

<a href="https://koso.ai">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/assets/koso-logo-white.svg">
    <img src="docs/assets/koso-logo.svg" alt="Koso" width="180">
  </picture>
</a>

# AI NEWS DAILY

**The day in AI, read for you. Scored, filtered and published every morning.**

[Read today's briefing](https://aashishpahwa.github.io/Horizon/) · [RSS](https://aashishpahwa.github.io/Horizon/feed-en.xml) · [koso.ai](https://koso.ai)

</div>

---

### `01` What it is

AI News Daily is an internal Koso pipeline that reads around a hundred AI sources every morning, scores each story out of 10 with an LLM, and publishes only the ones that clear the bar. No feed to scroll. One page a day, ranked, with background and sources on every story.

It runs entirely on GitHub Actions. There is no server to keep alive.

### `02` How it works

| | Step | What happens |
|---|---|---|
| `01` | **Collect** | Pulls the last 24 hours from 26 RSS feeds, Hacker News, GitHub releases and Telegram. |
| `02` | **Deduplicate** | Merges the same story arriving from different sources, then merges stories covering the same event. |
| `03` | **Score** | `gpt-4o-mini` rates every item from 0 to 10. Anything under 7 is dropped. |
| `04` | **Enrich** | Searches for related coverage and writes background, impact and community reaction for each kept story. |
| `05` | **Publish** | Commits the briefing, rebuilds the site on GitHub Pages and posts the summary to an n8n webhook. |

Runs daily at 04:00 UTC. If the AI provider rejects the key, the run fails loudly instead of publishing an empty page.

### `03` Sources

| Type | Examples |
|---|---|
| Labs and companies | OpenAI, Google AI, DeepMind, Hugging Face, NVIDIA, LangChain |
| Writers and newsletters | Simon Willison, Interconnects, Latent Space, Ahead of AI, SemiAnalysis |
| News | The Decoder, MIT Tech Review, IEEE Spectrum, VentureBeat |
| Community | Hacker News, r/MachineLearning, r/LocalLLaMA and five more subreddits |
| Code | GitHub Trending, releases from Ollama, llama.cpp, Transformers, LangChain, vLLM |

The full list lives in [`data/config.github.json`](data/config.github.json). Add a feed there and it is in tomorrow's briefing.

### `04` Run it yourself

```bash
uv sync
cp data/config.github.json data/config.json
OPENAI_API_KEY=sk-... uv run horizon --hours 24
```

Rebuild a missed day without notifying anyone:

```bash
uv run horizon --date 2026-10-18
```

On GitHub, the workflow needs two repository secrets: `OPENAI_API_KEY` and `N8N_WEBHOOK_URL`.

### `05` Repository

| Path | Purpose |
|---|---|
| `.github/workflows/daily-ai-news.yml` | The daily run: score, commit, deploy, notify. |
| `.github/workflows/upstream-sync.yml` | Weekly check for engine updates. Opens a PR, never merges on its own. |
| `data/config.github.json` | Sources, model, score threshold. |
| `docs/` | The briefing site: Jekyll, Koso layout. |
| `src/` | The pipeline. |

---

<div align="center">

**Built by [Koso](https://koso.ai)** · custom AI systems that ship work · for [Aashish Pahwa](https://aashishpahwa.com)

<sub>The collection and scoring engine is based on the open-source <a href="https://github.com/Thysrael/Horizon">Horizon</a> project, used under the MIT License.</sub>

</div>
