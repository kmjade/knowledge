---
tags: 
pare: area
---

> [!NOTE] 
> 长期责任或承诺，用于存储你关心的领域或主题，例如学习、工作、和生活。
## No. of Areas [[领域]] 🧠
```dataview
list without id length(rows.file.name)
from "2 Areas"
where para = "area"
group by 1
```

```dataview
TABLE WITHOUT ID file.link as "Area", length(file.inlinks) as "No. of Linked Files"
FROM "1 Projects" or "2 Areas" or "3 Resources"
WHERE para = "area"
SORT length(file.inlinks) desc
```

```dataview
TABLE domain 
FROM "2 Areas" 
SORT file.mtime desc 
LIMIT 10
```

> [!tldr]- Detailed
> ```dataview
> table file.inlinks as "Linked Files"
> from "2 Areas" 
> where para = "area"
> sort file.name
> ```
