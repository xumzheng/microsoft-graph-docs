---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ColumnDefinition()
request_body.required = True

request_body.hidden = False

request_body.propagate_changes = False




result = await client.sites_by_id('site-id').contentTypes_by_id('contentType-id').columns_by_id('columnDefinition-id').patch(request_body = request_body)


```