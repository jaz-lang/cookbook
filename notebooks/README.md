# JAZ tutorial notebooks

The hands-on tutorials for [jaz-lang.ai](https://jaz-lang.ai). Each notebook is
self-contained and runs in Google Colab — no local setup required.

| Notebook | Topic | Time |
| :------- | :---- | :--- |
| [01-quickstart.ipynb](01-quickstart.ipynb) | Your first agent: `jaz.invoke` and typed results | ~10 min |
| [02-tools-and-libraries.ipynb](02-tools-and-libraries.ipynb) | Give agents typed tools with `Library` | ~15 min |
| [03-recursive-agents.ipynb](03-recursive-agents.ipynb) | Nested agents and pool budgets | ~20 min |
| [04-hooks-and-tracing.ipynb](04-hooks-and-tracing.ipynb) | Logging, custom hooks, and tracing | ~20 min |

## Open in Colab

Colab opens any notebook in this repo directly from GitHub:

```
https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/<file>.ipynb
```

The website links to these via `src/data/tutorials.ts` in the `jaz-website` repo — keep that
list in sync when you add or rename a notebook.

## Running

Every notebook starts with a **Setup** section that installs the package and prompts for an
API key:

```python
%pip install -q jaz-lang
```

JAZ uses native OpenAI / Anthropic clients, so set `OPENAI_API_KEY` (or `ANTHROPIC_API_KEY`)
when prompted, or via Colab's secrets manager. The default model is set with
`jaz.configure(model_config={'model': 'openai/gpt-4o-mini'})` — change it to suit.
