---
layout: community_extension_doc
title: Community Extensions
excerpt: |
  List of Community contributed open-source DuckDB extension 
---

Welcome to the documentation for the DuckDB Community Extension Repository.
This website contains all documentation specific to community extensions.
For the core DuckDB database, check out the [DuckDB documentation](https://duckdb.org/docs/).

## What are Community Extensions

Community extensions are [DuckDB extensions]({% link docs/extensions/overview.md %}) that are not maintained by the DuckDB team.
They are different from the [core extensions]({% link docs/extensions/core_extensions.md %}), which *are* maintained by the DuckDB team.
Community extensions are distributed through the [Community Extension Repository](https://github.com/duckdb/community-extensions), where anyone building an open-source DuckDB extension can make Pull Requests to submit an extension.
Note that this makes DuckDB Community extensions conceptually very similar to a package manager such as [Homebrew](https://brew.sh/).

## How to Use a Community Extension

To install and load a community extension, simply run:

```sql
INSTALL ⟨extension_name⟩ FROM community;
LOAD ⟨extension_name⟩;
```

For example, to install and load the `quack` extension:

```sql
INSTALL quack FROM community;
LOAD quack;
```

The `quack` extension is now loaded and ready to use

```sql
SELECT quack('world');
```
