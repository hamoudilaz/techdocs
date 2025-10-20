# TechDocs

TechDocs is Backstage's documentation-as-code system.

## How it works

1. You write docs in Markdown.
2. MkDocs builds them into static HTML.
3. Backstage renders them inside the “Docs” tab of each component.

## Local Build

```bash
npx @techdocs/cli serve
```

## Configuration

In `app-config.yaml`:

```yaml
techdocs:
  builder: local
  generator:
    runIn: docker
  publisher:
    type: local
```
