# Temporal Example

**This example is incomplete.** It holds the shared repo setup, but no code yet.

## What it shows

The goal of this example is a small workflow on [Temporal](https://temporal.io). Temporal runs a workflow as durable code: when a worker stops, another worker continues the workflow from its last step.

## Run it

1. Install [mise](https://mise.jdx.dev/getting-started.html).
2. Install the tools and the hooks:

   ```bash
   git clone git@github.com:tabmadi/temporal-example.git
   cd temporal-example
   mise install
   mise run setup
   ```

## What is deliberately missing

- **The workflow**: no worker, workflow, or activity exists yet. This is what makes the example incomplete.

## Tasks

| Task | Does |
| --- | --- |
| `mise run setup` | Installs the git hooks |
| `mise run lint` | Runs `lint:md` and `lint:secrets` |
| `mise run check` | Runs `lint` and `test`. Run it before you finish a change |
| `mise run ci` | Runs exactly what CI runs. The `pre-push` hook runs it too |

## License

Apache License 2.0. See [LICENSE](LICENSE).
