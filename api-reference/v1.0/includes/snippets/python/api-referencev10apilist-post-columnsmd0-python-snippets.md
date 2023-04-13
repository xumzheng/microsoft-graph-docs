---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ColumnDefinition()
request_body.description = 'test'

request_body.enforce_unique_values = False

request_body.hidden = False

request_body.indexed = False

request_body.name = 'Title'

text = TextColumn()
text.allow_multiple_lines = False

text.append_changes_to_existing_text = False

text.lines_for_editing = 0

text.max_length = 255


request_body.text = text



result = await client.sites_by_id('site-id').lists_by_id('list-id').columns.post(request_body = request_body)


```