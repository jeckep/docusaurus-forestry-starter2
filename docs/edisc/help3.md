---
slug: help3
title: Fuzzy search / stemming / lemmatisation
---

### Fuzzy search
```
    content:roam~
```
This search will match terms like roams, foam, & foams. It will also match the word "roam" itself.
An optional distance parameter specifies the maximum number of edits allowed, between 0 and 2, defaulting to 2. For example

```
    content:roam~1
```
This will match terms like roams & foam - but not foams since it has an edit distance of "2".


### Stemming

Stemming is language specific algorithm. So in order to use it you should configure index before processing to make required stemming.
If index configured to make english stemming you are able to search (and configure keywords and custodians)
by stem in the document field 'stem_txt_en' like this:
```
    stem_txt_en:intend
```
This will return docs with words: intend, intended, intending etc. in content or name.

### Lemmatisation

Lemmatisation is language specific algorithm. It is supported only for english.
So in order to use it you should configure index before processing to make required lemmatization.
You should choose fields for lemmatisation. If for instance you choose name and content fields,
then you are able to query lemmatized new fields 'content_lem_en' and 'name_lem_en'.
