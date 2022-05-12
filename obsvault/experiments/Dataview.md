---
created: 2022-05-05T11:21:17-06:00
updated: 2022-05-05T11:21:17-06:00
---
# Dataview

```ad-tip
[Data Annotation - Dataview (blacksmithgu.github.io)](https://blacksmithgu.github.io/obsidian-dataview/data-annotation/#implicit-fields)

https://blacksmithgu.github.io/obsidian-dataview/data-annotation/#implicit-fields
```


---
## Sections
```dataview
TABLE WITHOUT ID
	file.folder AS Folder,
	file.link AS Name,
	file.tags AS Tags,	
	file.inlinks,
	file.outlinks,
	file.mtime AS Modified,
	file.size AS Size,
	url AS posting_url

FROM "career/sections"
SORT file.folder ASC, file.name ASC
```

### Not Used
```md
	file.path,	
	file.ctime,
	file.link,
	file.tasks
```


---
## Postings
```dataview
TABLE
	file.size,
	url AS posting_url
FROM "career/2022-04-14 Atlassian/postings"
SORT file.name ASC
```





---
## Also See
- Dataview queries in [[README - Greg Stevens for Atlassian#Job Postings I am Interested In]]
- [obsidian-dataview](https://blacksmithgu.github.io/obsidian-dataview/query/sources/)

