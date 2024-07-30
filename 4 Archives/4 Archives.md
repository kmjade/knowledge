---
tags: 
pare:
---

> [!NOTE]
> 已完成的项目、领域或资源，我不再需要或感兴趣

## No. of 档案 (Archives)  [[档案]]

```dataview
list without id length(rows.file.name)
from "4 Archive"
where para = "archives"
group by 1
```

```dataview
TABLE WITHOUT ID file.link as "Archive", length(file.inlinks) as "No. of Linked Files"
FROM "4 Archive"
WHERE para = "resource"
SORT length(file.inlinks) desc
```

> [!tldr]- Detailed
> ```dataview
> table file.inlinks as "Linked Files"
> from "3 Resources" 
> where para = "resource"
> sort file.name
> ```

 