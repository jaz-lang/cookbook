# JAZ tutorial notebooks

The hands-on tutorials for [jaz-lang.ai](https://jaz-lang.ai). Each notebook is
self-contained and runs in Google Colab — no local setup required.

| Notebook | Topic | Time |
| :------- | :---- | :--- |
| [01-inputs.ipynb](01-inputs.ipynb) | One kind of argument: prompts, tools, data and your own objects all go in the same way | ~10 min |
| [02-subagents-and-scope.ipynb](02-subagents-and-scope.ipynb) | Agents calling agents, why inputs stop at one call, and how `scope` reaches the whole tree | ~10 min |
| [03-hooks-events-and-effects.ipynb](03-hooks-events-and-effects.ipynb) | The extension model: typed returns, validation, budgets and limits are all one mechanism | ~12 min |
| [04-configuration.ipynb](04-configuration.ipynb) | The LLM, the REPL and the protocol underneath — including what the agent is allowed to import | ~10 min |
| [05-putting-it-together.ipynb](05-putting-it-together.ipynb) | One real analysis using all of it: a DataFrame in, a typed report with a chart out | ~12 min |

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
