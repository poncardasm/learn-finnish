# 😊 Positive Emotions

```dataview
table without id
	file.link as Word,
	en as English,
	pos as PoS,
	form as Form
where
	contains(category,this.file.link) and
	!contains(file.name, "Template")
sort file.name ASC
```
