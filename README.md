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
| [Inputs: prompts, tools, and data](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/01-inputs.ipynb) | One kind of argument: prompts, tools, data and your own objects all go in the same way | ~10 min |
| [Recursive subagents and scope](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/02-subagents-and-scope.ipynb) | Agents calling agents, why inputs stop at one call, and how `scope` reaches the whole tree | ~10 min |
| [Hooks, events and effects](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/03-hooks-events-and-effects.ipynb) | The extension model: typed returns, validation, budgets and limits are all one mechanism | ~12 min |
| [Configuration](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/04-configuration.ipynb) | The LLM, the REPL and the protocol underneath — including what the agent is allowed to import | ~10 min |
| [Putting it together](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/05-putting-it-together.ipynb) | The homepage's program, using all of it: a DataFrame and a web search in, a typed, checked report out | ~12 min |

Run them in order — each one builds on the last.

See [`notebooks/README.md`](notebooks/README.md) for how to run them.

## License

[Apache 2.0](LICENSE).
