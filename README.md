# JAZ Cookbook

Runnable notebooks, examples, and guides for the [JAZ](https://jaz-lang.ai) framework — a
Python framework for building and optimizing LLM agents through a code-first REPL loop.

This is the public home for JAZ's hands-on material. Install the package with
`pip install jaz-lang` (it imports as `jaz`).

## Contents

- [`notebooks/`](notebooks/) — Google Colab tutorials. Each runs in your browser, no local
  setup required, and each ships with its outputs so you can read it without running
  anything.

## Tutorials

| Notebook | What it covers | Time |
| :------- | :------------- | :--- |
| [Talk to your data](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/01-talk-to-your-data.ipynb) | Hand over a real DataFrame, get a typed report back, then watch the loop that produced it | ~10 min |
| [Inputs and tools](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/02-inputs-and-tools.ipynb) | Why your prompt, your data and your tools are one mechanism — and how to control what the model sees | ~10 min |
| [Subagents and scope](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/03-subagents-and-scope.ipynb) | Agents calling agents, why inputs stop at one call, and how `scope` reaches the whole tree | ~12 min |
| [Budgets and failure](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/04-budgets-and-failure.ipynb) | Caps that actually fire, retries you can watch, and the two ways a run fails | ~10 min |
| [Hooks and tracing](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/05-hooks-and-tracing.ipynb) | The extension model behind every limit you have used: events in, effects out | ~10 min |

Run them in order — each one builds on the last.

See [`notebooks/README.md`](notebooks/README.md) for how to run them.

## License

[Apache 2.0](LICENSE).
