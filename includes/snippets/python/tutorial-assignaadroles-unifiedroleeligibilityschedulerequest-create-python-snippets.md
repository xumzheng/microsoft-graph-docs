---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.setAction(UnifiedRoleScheduleRequestActions('adminassign'))

request_body.setJustification('Assign User Admin eligibility to IT Helpdesk (User) group')

request_body.setRoleDefinitionId('fe930be7-5e62-47db-91af-98c3a49a38b1')

request_body.setDirectoryScopeId('/')

request_body.setPrincipalId('e77cbb23-0ff2-4e18-819c-690f58269752')

scheduleInfo = RequestSchedule()
scheduleInfo.setStartDateTime(DateTime('2021-07-01T00:00:00Z'))

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.setEndDateTime(DateTime('2022-06-30T00:00:00Z'))

scheduleInfoExpiration.setType(ExpirationPatternType('afterdatetime'))


scheduleInfo.setExpiration($scheduleInfoExpiration)

request_body.setScheduleInfo($scheduleInfo)


result = await client.roleManagement_directory_roleEligibilityScheduleRequests.post(request_body)


```