---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.Action(UnifiedRoleScheduleRequestActions('adminassign'))

request_body.justification = 'Assign Groups Admin to IT Helpdesk group'

request_body.roleDefinitionId = 'fdd7a751-b60b-444a-984c-02652fe8fa1c'

request_body.directoryScopeId = '/'

request_body.principalId = '071cc716-8147-4397-a5ba-b2105951cc0b'

scheduleInfo = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2022-04-10T00:00:00Z')

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.Type(ExpirationPatternType('noexpiration'))


scheduleInfo.expiration = scheduleInfoExpiration

request_body.scheduleInfo = scheduleInfo



result = await client.roleManagement.directory.roleAssignmentScheduleRequests.post(request_body = request_body)


```