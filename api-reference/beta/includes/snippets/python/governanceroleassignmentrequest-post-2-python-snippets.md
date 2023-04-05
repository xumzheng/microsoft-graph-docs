---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GovernanceRoleAssignmentRequest()
request_body.setRoleDefinitionId('8b4d1d51-08e9-4254-b0a6-b16177aae376')

request_body.setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5')

request_body.setSubjectId('918e54be-12c4-4f4c-a6d3-2ee0e3661c51')

request_body.setAssignmentState('Active')

request_body.setType('UserAdd')

request_body.setReason('Activate the owner role')

schedule = GovernanceSchedule()
schedule.setType('Once')

schedule.setStartDateTime(DateTime('2018-05-12T23:28:43.537Z'))

$schedule.setDuration( \DateInterval('PT9H'))


request_body.setSchedule($schedule)
request_body.setLinkedEligibleRoleAssignmentId('e327f4be-42a0-47a2-8579-0a39b025b394')



result = await client.privilegedAccessById('privilegedAccess-id').roleAssignmentRequests.post(request_body)


```