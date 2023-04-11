---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddCopyPostRequestBody()
request_body.contentType = 'https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101'



request_configuration = AddCopyRequestBuilderPostRequestConfiguration(
)


result = await client.sites_by_id('site-id').lists_by_id('list-id').contentTypes.addCopy.post(request_body = request_body)


```