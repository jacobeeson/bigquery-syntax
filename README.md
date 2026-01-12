# BigQuery Syntax

Accurate syntax highlighting for BigQuery Standard SQL.

[![Version](https://img.shields.io/badge/version-1.2.1-blue)](https://marketplace.visualstudio.com/items?itemName=jacobeeson.bigquery-syntax) [![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.txt)

## Features

- **BigQuery Standard SQL** — Full support for modern syntax (not Legacy SQL)
- **490+ functions** — AI, ML, window functions, aggregates, geography, JSON, arrays, strings, math, and more
- **Code folding** — Collapse BEGIN/END blocks, CASE expressions, CTEs, and function definitions
- **All data types** — INT64, STRING, ARRAY, STRUCT, JSON, GEOGRAPHY, RANGE, and all numeric/temporal types
- **String variants** — Single, double, raw (`r''`), bytes (`b''`), multi-line (`'''`), and combinations
- **BigQuery identifiers** — Backticks, parameters (`@param`), system variables (`@@project_id`)
- **All comment styles** — `--`, `#`, and `/* */`

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

## Usage

BigQuery syntax highlighting activates automatically for `.bq` and `.bqsql` files.

**For `.sql` files:** Configure file associations (see above) or manually select the language:
1. Open your `.sql` file
2. Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac)
3. Type "Change Language Mode"
4. Select "BigQuery SQL"

**Code Folding:** Click the collapse arrows next to BEGIN/END blocks, CASE expressions, CTEs, and function definitions to fold code sections.

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

## Why This Extension?

**Comprehensive Coverage:**
- **490+ functions** - Most complete BigQuery function library available
- **Latest features** - AI.*, ML.*, OBJ.* functions from January 2026 release
- **Quarterly updates** - Synchronized with Google's BigQuery feature releases

**BigQuery-Specific Syntax:**
- System variables: `@@project_id`, `@@dataset_id`, `@@time_zone`
- Pseudo-columns: `_TABLE_SUFFIX`, `_PARTITIONTIME`, `_PARTITIONDATE`
- Time travel: `FOR SYSTEM_TIME AS OF`
- Scripting: `BEGIN/END`, `EXCEPTION`, `LOOP`, `DECLARE`
- String variants: Raw strings (`r''`), bytes (`b''`), multi-line (`'''`)

**Better Than Alternatives:**
- Generic SQL extensions miss BigQuery-specific constructs
- Other BigQuery extensions have incomplete function coverage or outdated syntax
- This extension is actively maintained with test-driven development

## License

MIT License - see [LICENSE.txt](LICENSE.txt) for full details.

Copyright © 2026 jacobeeson
