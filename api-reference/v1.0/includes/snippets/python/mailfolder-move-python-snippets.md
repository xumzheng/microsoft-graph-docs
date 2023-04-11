---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MovePostRequestBody()
request_body.destinationId = 'destinationId-value'



request_configuration = MoveRequestBuilderPostRequestConfiguration(
)


result = await client.me.mailFolders_by_id('mailFolder-id').move.post(request_body = request_body)


```