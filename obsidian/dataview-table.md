### Table without ID

```md
table without id
	file.link as Title,
	status as Status,
	created as Created,
	tags as Tags
where
	contains(status, "published") and
	contains(category,this.file.link) and
	!contains(file.name, "Template")
sort date asc
```

