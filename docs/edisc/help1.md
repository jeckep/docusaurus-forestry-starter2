---
slug: help1
title: Advanced case config
---

## Examples

*Return all docs contain a word "test", case insensitive (dosc with tEst, TEST and other will be also in the result)*
```
    content:"test"
```

*Return all docs contain a word "Test", case sensitive.*
```
    content_cs:"Test"
```

*Return all docs contain a word "test" in content or on name, case insensitive.*
```
    content:"Test" name:"test"
```
