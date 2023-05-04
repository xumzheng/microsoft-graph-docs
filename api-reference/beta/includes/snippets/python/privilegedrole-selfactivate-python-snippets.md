---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Self_activate_post_request_body()
request_body.reason = 'reason-value'

request_body.duration = 'duration-value'

request_body.ticket_number = 'ticketNumber-value'

request_body.ticket_system = 'ticketSystem-value'




result = await client.privileged_roles.by_privileged_role_id('privilegedRole-id').self_activate.post(request_body = request_body)


```