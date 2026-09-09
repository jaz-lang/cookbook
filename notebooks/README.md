# JAZ tutorial notebooks

The hands-on tutorials for [jaz-lang.ai](https://jaz-lang.ai). Each notebook is
self-contained and runs in Google Colab — no local setup required.

| Notebook | Topic | Time |
| :------- | :---- | :--- |
| [talk-to-your-data.ipynb](talk-to-your-data.ipynb) | Pass a DataFrame straight in, get back a typed report | ~5 min |
| [01-quickstart.ipynb](01-quickstart.ipynb) | Your first agent: `jaz.invoke` and typed results | ~10 min |
| [02-custom-tools.ipynb](02-custom-tools.ipynb) | Give agents typed tools (plain Python functions) | ~15 min |
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

JAZ routes to providers through LiteLLM, so set `OPENAI_API_KEY` (or `ANTHROPIC_API_KEY`)
when prompted, or via Colab's secrets manager. The model is set with
`jaz.configure(llm=LiteLLM(model='openai/gpt-5.4-nano'))` (import `LiteLLM` from `jaz.llm`) —
change it to suit.
