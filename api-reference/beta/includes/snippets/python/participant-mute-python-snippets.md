---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MutePostRequestBody()
request_body.setClientContext('d45324c1-fcb5-430a-902c-f20af696537c')



result = await client.communications.callsby_id('call-id').participantsby_id('participant-id').mute.post(request_body)


```