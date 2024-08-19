# Super Carnival

This is a cool tool that does useful things.

## Usage

    curl --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/petite-surgeonfish/super-carnival/main/run.sh | sh

or to use a specific version:

    curl --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/petite-surgeonfish/super-carnival/{COMMIT ID}/run.sh | sh

## GitHub Actions

```yaml
on: [push]

jobs:
  example_job:
    runs-on: ubuntu-latest
    name: An example job
    steps:
      - uses: petite-surgeonfish/super-carnival@main
```

or pin to a specific version:

```yaml
on: [push]

jobs:
  example_job:
    runs-on: ubuntu-latest
    name: An example job
    steps:
      - uses: petite-surgeonfish/super-carnival@{COMMIT ID}
```
