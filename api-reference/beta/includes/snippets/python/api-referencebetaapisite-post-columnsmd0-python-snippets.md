---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ColumnDefinition()
request_body.description = 'test'

request_body.enforceUniqueValues = false

request_body.hidden = false

request_body.indexed = false

request_body.name = 'Title'

text = TextColumn()
text.allowMultipleLines = false

text.appendChangesToExistingText = false

text.linesForEditing = 0

text.maxLength = 255


request_body.text = text



result = await client.sites_by_id('site-id').columns.post(request_body = request_body)


```