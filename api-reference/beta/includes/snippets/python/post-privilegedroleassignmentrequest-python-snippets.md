---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Privileged_role_assignment_request()
request_body.duration = '2'

request_body.reason = 'Activate the role for business purpose'

request_body.ticket_number = '234'

request_body.ticket_system = 'system'

schedule = Governance_schedule()
schedule.startDateTime = DateTime('2018-02-08T02:35:17.903Z')


request_body.schedule = schedule
request_body.type = 'UserAdd'

request_body.assignment_state = 'Active'

request_body.role_id = '88d8e3e3-8f55-4a1e-953a-9b9898b8876b'




result = await client.privileged_role_assignment_requests.post(request_body = request_body)


```