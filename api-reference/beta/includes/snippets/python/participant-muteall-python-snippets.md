---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MuteAllPostRequestBody()
request_body.setParticipants(['', ])

request_body.setClientContext('clientContext-value')



result = await client.communications_callsby_id('call-id')_participants_muteAll.post(request_body)


```