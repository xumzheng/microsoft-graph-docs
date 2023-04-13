---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.Action(UnifiedRoleScheduleRequestActions('adminassign'))

request_body.justification = 'Assign User Admin eligibility to IT Helpdesk (User) group'

request_body.roleDefinitionId = 'fe930be7-5e62-47db-91af-98c3a49a38b1'

request_body.directoryScopeId = '/'

request_body.principalId = 'e77cbb23-0ff2-4e18-819c-690f58269752'

schedule_info = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2021-07-01T00:00:00Z')

schedule_info_expiration = ExpirationPattern()
scheduleInfoExpiration.endDateTime = DateTime('2022-06-30T00:00:00Z')

scheduleInfoExpiration.Type(ExpirationPatternType('afterdatetime'))


scheduleInfo.expiration = scheduleInfoExpiration

request_body.schedule_info = scheduleInfo



result = await client.roleManagement.directory.roleEligibilityScheduleRequests.post(request_body = request_body)


```