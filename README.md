# BigQuery Syntax

Accurate syntax highlighting for BigQuery Standard SQL.

[![VS Code Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/jacobeeson.bigquery-syntax)](https://marketplace.visualstudio.com/items?itemName=jacobeeson.bigquery-syntax)
[![VS Code Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/jacobeeson.bigquery-syntax)](https://marketplace.visualstudio.com/items?itemName=jacobeeson.bigquery-syntax)

## Features

- **BigQuery Standard SQL** — Full support for modern BigQuery syntax (not Legacy SQL)
- **~490 functions** across 20 categories including AI, aggregates, window functions, geography, JSON, ML, object storage, and more
- **All data types** — INT64, FLOAT64, NUMERIC, BIGNUMERIC, STRING, BYTES, DATE, TIME, DATETIME, TIMESTAMP, INTERVAL, ARRAY, STRUCT, JSON, GEOGRAPHY, RANGE
- **String literals** — Single, double, triple-quoted, raw (`r''`), bytes (`b''`), and combinations (`rb''`, `br''`)
- **Parameters** — Named (`@param`) and system variables (`@@project_id`, `@@dataset_id`)
- **Identifiers** — Backtick-quoted identifiers with full Unicode support
- **Comments** — All styles: `--`, `#`, and `/* */`

## File Associations

### Automatic

Files with these extensions are automatically recognized:
- `.bq`
- `.bqsql`

### Manual (.sql files)

To associate `.sql` files with BigQuery syntax, add to your `settings.json`:

```json
{
  "files.associations": {
    "*.sql": "bigquery"
  }
}
```

Or for specific paths only:

```json
{
  "files.associations": {
    "**/bigquery/**/*.sql": "bigquery"
  }
}
```

## Installation

### VS Code Marketplace

1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Search for "BigQuery Syntax"
4. Click Install

Or install directly: [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=jacobeeson.bigquery-syntax)

### Manual Install

1. Download the `.vsix` file from [Releases](https://github.com/jacobeeson/bigquery-syntax/releases)
2. In VS Code: Extensions → ⋯ → Install from VSIX...

## Comparison

This extension provides more comprehensive coverage than alternatives:
- Actively maintained with current BigQuery syntax
- Covers newer features: AI functions, RANGE types, KLL functions, DLP functions, vector distance functions
- Proper handling of all string literal variants and escape sequences

## Contributing

Issues and pull requests are welcome.

[GitHub Repository](https://github.com/jacobeeson/bigquery-syntax)

## License

MIT
