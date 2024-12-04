---
tags: 
pare: archive
---

> [!NOTE]
> 已完成的项目、领域或资源，我不再需要或感兴趣项目

## No. of 档案 (Archives)  [[档案]]
```dataview
list without id length(rows.file.name)
from "4 Archives"
where para = "archive"
group by 1
```

```dataview
TABLE WITHOUT ID file.link as "Archive", length(file.inlinks) as "No. of Linked Files"
FROM "4 Archives"
WHERE para = "archive"
SORT length(file.inlinks) desc
```

> [!tldr]- Detailed
> ```dataview
> table file.inlinks as "Linked Files"
> from "4 Archives" 
> where para = "archive"
> sort file.name
> ```

 