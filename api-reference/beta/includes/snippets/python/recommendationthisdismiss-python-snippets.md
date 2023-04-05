---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DismissPostRequestBody()
request_body.setDismissReason('Recommendations is not relevant for my organization because...')



result = await client.directory_recommendationsby_id('recommendation-id')_dismiss.post(request_body)


```