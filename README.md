# nextversion
GitHub Actions to get the next version from tag.

# Usage

```yml
steps:
- uses: swiftty/nextversion@v0.0.0
  with: 
    bump: patch
```

## Inputs

| Input      | Description                                               | Default      |
|------------|-----------------------------------------------------------|--------------|
| bump       | The next version from tag or `from`. `patch｜minor｜major`. | **Required** |
| from       | The current version, for uses manually.                   | None         |
| tag_prefix | Find tag name with prefix. eg.) `v` or ...                | `''`         |

## Outputs

| Output | Description                                                           |
|--------|-----------------------------------------------------------------------|
| next   | The next version specified by `bump` target, with added `tag_prefix`. |