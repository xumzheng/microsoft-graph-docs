---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedRoleAssignmentRequest()
request_body.duration = '2'

request_body.reason = 'Activate the role for business purpose'

request_body.ticketNumber = '234'

request_body.ticketSystem = 'system'

schedule = GovernanceSchedule()
schedule.startDateTime = DateTime('2018-02-08T02:35:17.903Z')


request_body.schedule = schedule
request_body.type = 'UserAdd'

request_body.assignmentState = 'Active'

request_body.roleId = '88d8e3e3-8f55-4a1e-953a-9b9898b8876b'




result = await client.privilegedRoleAssignmentRequests.post(request_body = request_body)


```