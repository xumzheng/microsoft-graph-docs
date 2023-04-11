---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddCopyFromContentTypeHubPostRequestBody()
request_body.contentTypeId = '0x0101'




result = await client.sites_by_id('site-id').lists_by_id('list-id').contentTypes.addCopyFromContentTypeHub.post(request_body = request_body)


```