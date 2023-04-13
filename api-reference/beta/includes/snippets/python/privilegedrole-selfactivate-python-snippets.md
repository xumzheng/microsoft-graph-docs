---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SelfActivatePostRequestBody()
request_body.reason = 'reason-value'

request_body.duration = 'duration-value'

request_body.ticketNumber = 'ticketNumber-value'

request_body.ticketSystem = 'ticketSystem-value'




result = await client.privilegedRoles_by_id('privilegedRole-id').selfActivate.post(request_body = request_body)


```