---
created: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
modified: <% tp.file.last_modified_date("YYYY-MM-DDTHH:mm:ss") %>
tags:
  - elder_scrolls_online
  - location
---
```dataview
list
from "ESO/Locations"
where contains(type, "location")
```
