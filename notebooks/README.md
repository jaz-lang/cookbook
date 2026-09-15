# JAZ tutorial notebooks

The hands-on tutorials for [jaz-lang.ai](https://jaz-lang.ai). Each notebook is
self-contained and runs in Google Colab — no local setup required.

| Notebook | Topic | Time |
| :------- | :---- | :--- |
| [01-talk-to-your-data.ipynb](01-talk-to-your-data.ipynb) | Hand over a real DataFrame, get a typed report, then watch the loop | ~10 min |
| [02-inputs-and-tools.ipynb](02-inputs-and-tools.ipynb) | One mechanism for prompt, data and tools; controlling what the model sees | ~10 min |
| [03-subagents-and-scope.ipynb](03-subagents-and-scope.ipynb) | Agents calling agents, and why `scope` exists | ~12 min |
| [04-budgets-and-failure.ipynb](04-budgets-and-failure.ipynb) | Caps that fire, retries you can watch, and how runs fail | ~10 min |
| [05-hooks-and-tracing.ipynb](05-hooks-and-tracing.ipynb) | Events in, effects out — the model behind every limit | ~10 min |

Run them in order; each builds on the one before. Every notebook is committed with its outputs, so you can read the whole sequence without an API key.

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
