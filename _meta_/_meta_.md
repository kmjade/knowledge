---
pare: _meta_
---

```dataview
LIST FROM "_meta_"
WHERE !contains(file.name, "archive") AND file.name != "_meta_"
```