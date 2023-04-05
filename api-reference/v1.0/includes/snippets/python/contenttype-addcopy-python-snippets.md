---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddCopyPostRequestBody()
request_body.setContentType('https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101')



result = await client.sitesby_id('site-id').listsby_id('list-id').contentTypes.addCopy.post(request_body)


```