---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Make_permanent_post_request_body()
request_body.reason = 'reason-value'

request_body.ticket_number = 'ticketNumber-value'

request_body.ticket_system = 'ticketSystem-value'




result = await client.privileged_role_assignments.by_privileged_role_assignment_id('privilegedRoleAssignment-id').make_permanent.post(request_body = request_body)


```