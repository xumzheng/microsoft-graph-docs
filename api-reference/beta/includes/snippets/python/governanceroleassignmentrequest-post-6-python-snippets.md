---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GovernanceRoleAssignmentRequest()
request_body.setRoleDefinitionId('0e88fd18-50f5-4ee1-9104-01c3ed910065')

request_body.setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5')

request_body.setSubjectId('74765671-9ca4-40d7-9e36-2f4a570608a6')

request_body.setAssignmentState('Eligible')

request_body.setType('AdminExtend')

request_body.setReason('extend role assignment')

schedule = GovernanceSchedule()
schedule.setType('Once')

schedule.setStartDateTime(DateTime('2018-05-12T23:53:55.327Z'))

schedule.setEndDateTime(DateTime('2018-08-10T23:53:55.327Z'))


request_body.setSchedule($schedule)


result = await client.privilegedAccessById('privilegedAccess-id').roleAssignmentRequests.post(request_body)


```