---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ColumnDefinition()
request_body.setDescription('test')

request_body.setEnforceUniqueValues(false)

request_body.setHidden(false)

request_body.setIndexed(false)

request_body.setName('Title')

text = TextColumn()
text.setAllowMultipleLines(false)

text.setAppendChangesToExistingText(false)

text.setLinesForEditing(0)

text.setMaxLength(255)


request_body.setText($text)


result = await client.sites_by_id('site-id').columns.post(request_body, headers=)


```