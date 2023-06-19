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

```xml reference title="/etc/clickhouse-server/users.d/allow-named-collections.xml"
https://github.com/ClickHouse/ClickHouse/blob/fd5dd103b30aaee6d7a4e7ff56d88448bea6e2f6/tests/integration/test_async_insert_memory/configs/users.xml#L3-L9
```

This next block is the same content, but it is copied and pasted into the markdown page.  The
rendered HTML is exactly the same except for the missing link to the full file.

```xml title="/etc/clickhouse-server/users.d/allow-named-collections.xml"
        <default>
            <password></password>
            <profile>default</profile>
            <quota>default</quota>
            <named_collection_control>1</named_collection_control>
            <show_named_collections_secrets>1</show_named_collections_secrets>
        </default>
```

