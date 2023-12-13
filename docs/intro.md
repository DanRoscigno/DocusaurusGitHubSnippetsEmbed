---
sidebar_position: 1
---

# Embedding snippets of code from GitHub

This first block is a section of lines from a configuration file used in an integration
test.  The URL used is to a particular commit for two reasons:
- Line numbers can change, referring to a specific commit guarantees that the line numbers
will stay correct.
- At some point we may have versioned docs; this allows us to link to the docs at the appropriate point in time.

The plan is to have dedicated tests for code that is included in the docs so that we know before the community when:
- a change happens to a dataset that is used in the docs
- a breaking change breaks a tutorial

```bash reference title="be.conf"
https://github.com/StarRocks/starrocks/blob/bed907747e07cd529a3b11e372997a14fd03436e/conf/be.conf#L21-L26
```

```sql reference title="JOIN from Quick Start"
https://github.com/StarRocks/starrocks/blob/878ed8ae56ded2324c90f52c5ea99e2d2abcb51a/docs/en/assets/quick-start/_SQL.mdx#L136-L147
```

