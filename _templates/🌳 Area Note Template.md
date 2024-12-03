<%*
const AREA_PATH = "/2 Areas/";
const AREA_SUGGESTION = tp.user.getAreaList();
area = await tp.system.suggester(AREA_SUGGESTION, tp.user.getAreaListValue(), false, "Area");
path = AREA_PATH + area + "/" + tp.file.title;
await tp.file.move(path);
-%>
---
tags: 
pare: 
sub_pare: 
note:
domain: 
  - "[[<% area %>]]"
creation date: <% tp.file.creation_date() %>
due_date: 
start_date: 
scheduled_date: 

---
## <% tp.file.title %>

