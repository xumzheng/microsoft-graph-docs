---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = List()
request_body.display_name = 'Books'

columns_column_definition1 = Column_definition()
columns_column_definition1.name = 'Author'

columns_column_definition1text = Text_column()

columns_column_definition1.text = columns_column_definition1text

columnsArray []= columnsColumnDefinition1;
columns_column_definition2 = Column_definition()
columns_column_definition2.name = 'PageCount'

columns_column_definition2number = Number_column()

columns_column_definition2.number = columns_column_definition2number

columnsArray []= columnsColumnDefinition2;
request_body.columns(columnsArray)


list = List_info()
list.template = 'genericList'


request_body.list = list



result = await client.sites.by_site_id('site-id').lists.post(request_body = request_body)


```