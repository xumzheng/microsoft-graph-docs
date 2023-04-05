---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GovernanceRoleAssignmentRequest()
request_body.setRoleDefinitionId('70521f3e-3b95-4e51-b4d2-a2f485b02103')

request_body.setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5')

request_body.setSubjectId('1566d11d-d2b6-444a-a8de-28698682c445')

request_body.setAssignmentState('Eligible')

request_body.setType('AdminUpdate')

schedule = GovernanceSchedule()
schedule.setType('Once')

schedule.setStartDateTime(DateTime('2018-03-08T05:42:45.317Z'))

schedule.setEndDateTime(DateTime('2018-06-05T05:42:31.000Z'))


request_body.setSchedule($schedule)


result = await client.privilegedAccess_by_id('privilegedAccess-id').roleAssignmentRequests.post(request_body)


```