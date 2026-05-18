# amlmarketplaces/langchain

Claude Code marketplace federating all `@amlplugins/langchain-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-langchain": {
      "source": { "source": "github", "repo": "amlmarketplaces/langchain" }
    }
  },
  "enabledPlugins": {
      "langchain-anthropic@aml-langchain": true,
      "langchain-aws@aml-langchain": true,
      "langchain-cohere@aml-langchain": true,
      "langchain-community@aml-langchain": true,
      "langchain-core@aml-langchain": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/langchain`, cached under `~/.claude/plugins/cache/aml-langchain/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (14 total)

- `langchain-anthropic` — [@amlplugins/langchain-anthropic](https://github.com/amlplugins/langchain-anthropic)
- `langchain-aws` — [@amlplugins/langchain-aws](https://github.com/amlplugins/langchain-aws)
- `langchain-cohere` — [@amlplugins/langchain-cohere](https://github.com/amlplugins/langchain-cohere)
- `langchain-community` — [@amlplugins/langchain-community](https://github.com/amlplugins/langchain-community)
- `langchain-core` — [@amlplugins/langchain-core](https://github.com/amlplugins/langchain-core)
- `langchain-google-genai` — [@amlplugins/langchain-google-genai](https://github.com/amlplugins/langchain-google-genai)
- `langchain-google-vertexai` — [@amlplugins/langchain-google-vertexai](https://github.com/amlplugins/langchain-google-vertexai)
- `langchain-groq` — [@amlplugins/langchain-groq](https://github.com/amlplugins/langchain-groq)
- `langchain-langgraph` — [@amlplugins/langchain-langgraph](https://github.com/amlplugins/langchain-langgraph)
- `langchain-meta` — [@amlplugins/langchain-meta](https://github.com/amlplugins/langchain-meta)
- `langchain-mistralai` — [@amlplugins/langchain-mistralai](https://github.com/amlplugins/langchain-mistralai)
- `langchain-ollama` — [@amlplugins/langchain-ollama](https://github.com/amlplugins/langchain-ollama)
- `langchain-openai` — [@amlplugins/langchain-openai](https://github.com/amlplugins/langchain-openai)
- `langchain-pinecone` — [@amlplugins/langchain-pinecone](https://github.com/amlplugins/langchain-pinecone)

## Related

- npm packages: `@amlplugins/langchain-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
