---
tags: 
pare:
---

> [!NOTE]
> 短期努力具有确定目标

## No. of Projects [[项目]]

```dataview
list without id length(rows.file.name)
from "1 Projects"
where para = "project"
group by 1
```

```dataview
TABLE WITHOUT ID file.link as "Projects", length(file.inlinks) as "No. of Linked Files"
FROM "1 Projects" or "2 Areas" or "3 Resources"
WHERE para = "project"
SORT length(file.inlinks) desc
```

> [!tldr]- Detailed
> ```dataview
> table file.inlinks as "Linked Files"
> from "1 Projects" 
> where para = "project"
> sort file.name
> ```

