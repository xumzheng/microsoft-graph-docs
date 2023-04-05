---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkPosition()
request_body.setIsCurrent(true)



result = await client.me.profile.positionsby_id('workPosition-id').patch(request_body)


```