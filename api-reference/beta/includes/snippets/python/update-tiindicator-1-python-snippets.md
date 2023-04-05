---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TiIndicator()
request_body.setDescription('description-updated')



result = await client.security.tiIndicatorsby_id('tiIndicator-id').patch(request_body)


```