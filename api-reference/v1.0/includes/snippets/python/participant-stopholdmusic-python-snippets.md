---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = StopHoldMusicPostRequestBody()
request_body.setClientContext('d45324c1-fcb5-430a-902c-f20af696537c')



result = await client.communications.calls._by_id('call-id').participants._by_id('participant-id').stopHoldMusic.post(request_body)


```