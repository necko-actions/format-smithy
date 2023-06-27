# Format Smithy models

This action allows users to format Smithy models using the Smithy CLI command: `smithy format`

## Basic usage

See [action.yml](action.yml)

Format all file in the current working directory :

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: necko-actions/format-smithy@v1
    with:
      version: "1.33.0"
```

Change the path in the current working directory, e.g, the directory `model` :

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: necko-actions/format-smithy@v1
    with:
      version: "1.33.0"
      path: "model"
```

