---
tags: 
pare: project
---

> [!NOTE]
> 短期努力具有确定目标，例如任务清单、进度报告、和结果总结。

## No. of Projects [[项目]]

```dataview
list without id length(rows.file.name)
from "1 Projects"
where pare = "project"
group by 1
```

```dataview
Table without id domain as "Area", sort(rows.file.link) as Projects
FROM "1 Projects"
WHERE file.name != "1 Projects" and contains(para, "project")
FLATTEN domain
GROUP BY domain
SORT domain
```

```dataview 
table start_date, by-when, status from "1 Projects"
SORT file.mtime desc
LIMIT 10
```
