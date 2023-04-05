---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyPostRequestBody()
request_body.setDestinationId('destinationId-value')



result = await client.me.mailFolders._by_id('mailFolder-id').copy.post(request_body)


```