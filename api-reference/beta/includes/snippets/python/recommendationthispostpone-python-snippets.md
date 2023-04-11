---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PostponePostRequestBody()
request_body.postponeUntilDateTime = DateTime('2023-02-01T02:53:00Z')



request_configuration = PostponeRequestBuilderPostRequestConfiguration(
)


result = await client.directory.recommendations_by_id('recommendation-id').postpone.post(request_body = request_body)


```