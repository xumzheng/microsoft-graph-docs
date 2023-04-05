---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GovernanceRoleAssignmentRequest()
request_body.setRoleDefinitionId('ea48ad5e-e3b0-4d10-af54-39a45bbfe68d')

request_body.setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5')

request_body.setSubjectId('918e54be-12c4-4f4c-a6d3-2ee0e3661c51')

request_body.setAssignmentState('Eligible')

request_body.setType('AdminAdd')

request_body.setReason('Assign an eligible role')

schedule = GovernanceSchedule()
schedule.setStartDateTime(DateTime('2018-05-12T23:37:43.356Z'))

schedule.setEndDateTime(DateTime('2018-11-08T23:37:43.356Z'))

schedule.setType('Once')


request_body.setSchedule($schedule)


result = await client.privilegedAccess._by_id('privilegedAccess-id').roleAssignmentRequests.post(request_body)


```