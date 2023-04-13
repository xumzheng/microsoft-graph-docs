---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.Action(UnifiedRoleScheduleRequestActions('adminassign'))

request_body.justification = 'Assign Attribute Assignment Admin eligibility to restricted user'

request_body.roleDefinitionId = '8424c6f0-a189-499e-bbd0-26c1753c96d4'

request_body.directoryScopeId = '/'

request_body.principalId = '071cc716-8147-4397-a5ba-b2105951cc0b'

schedule_info = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2022-04-10T00:00:00Z')

schedule_info_expiration = ExpirationPattern()
scheduleInfoExpiration.Type(ExpirationPatternType('afterdatetime'))

scheduleInfoExpiration.endDateTime = DateTime('2024-04-10T00:00:00Z')


scheduleInfo.expiration = scheduleInfoExpiration

request_body.schedule_info = scheduleInfo



result = await client.roleManagement.directory.roleEligibilityScheduleRequests.post(request_body = request_body)


```