---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyPostRequestBody()
request_body.setDestinationId('destinationId-value')



result = await client.me.messages_by_id('message-id').copy.post(request_body, headers=)


```