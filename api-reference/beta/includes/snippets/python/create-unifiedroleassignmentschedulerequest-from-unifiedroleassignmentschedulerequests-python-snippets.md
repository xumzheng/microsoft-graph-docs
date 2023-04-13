---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.action = 'AdminAssign'

request_body.justification = 'Assign User Admin to IT Helpdesk (User) group'

request_body.roleDefinitionId = 'fdd7a751-b60b-444a-984c-02652fe8fa1c'

request_body.directoryScopeId = '/'

request_body.principalId = '07706ff1-46c7-4847-ae33-3003830675a1'

schedule_info = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2021-07-01T00:00:00Z')

schedule_info_expiration = ExpirationPattern()
scheduleInfoExpiration.Type(ExpirationPatternType('noexpiration'))


scheduleInfo.expiration = scheduleInfoExpiration

request_body.schedule_info = scheduleInfo



result = await client.roleManagement.directory.roleAssignmentScheduleRequests.post(request_body = request_body)


```