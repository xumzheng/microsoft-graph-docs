---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = List()
request_body.displayName = 'Books'

columns_column_definition1 = ColumnDefinition()
columnsColumnDefinition1.name = 'Author'

columns_column_definition1_text = TextColumn()

columnsColumnDefinition1.text = columnsColumnDefinition1Text

columnsArray []= columnsColumnDefinition1;
columns_column_definition2 = ColumnDefinition()
columnsColumnDefinition2.name = 'PageCount'

columns_column_definition2_number = NumberColumn()

columnsColumnDefinition2.number = columnsColumnDefinition2Number

columnsArray []= columnsColumnDefinition2;
request_body.columns(columnsArray)


list = ListInfo()
list.template = 'genericList'


request_body.list = list



result = await client.sites_by_id('site-id').lists.post(request_body = request_body)


```