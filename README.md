# JAZ Cookbook

Runnable notebooks, examples, and guides for the [JAZ](https://jaz-lang.ai) framework — a
Python framework for building and optimizing LLM agents through a code-first REPL loop.

This is the public home for JAZ's hands-on material. Install the package with
`pip install jaz-lang` (it imports as `jaz`).

## Contents

- [`notebooks/`](notebooks/) — Google Colab tutorials. Each runs in your browser, no local
  setup required.

## Tutorials

| Notebook | Topic | Time |
| :------- | :---- | :--- |
| [Talk to your data](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/talk-to-your-data.ipynb) | Pass a DataFrame straight in, get back a typed report | ~5 min |
| [Your first agent](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/01-quickstart.ipynb) | `jaz.invoke` and typed results | ~10 min |
| [Custom tools](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/02-custom-tools.ipynb) | Typed tools (plain Python functions) | ~15 min |
| [Recursive agents & budgets](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/03-recursive-agents.ipynb) | Nested agents and pool budgets | ~20 min |
| [Observability with hooks](https://colab.research.google.com/github/jaz-lang/cookbook/blob/main/notebooks/04-hooks-and-tracing.ipynb) | Logging, custom hooks, tracing | ~20 min |

See [`notebooks/README.md`](notebooks/README.md) for how to run them.

## License

[Apache 2.0](LICENSE).
