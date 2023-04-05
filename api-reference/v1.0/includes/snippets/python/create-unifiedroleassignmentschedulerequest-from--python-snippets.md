---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.setAction(UnifiedRoleScheduleRequestActions('adminassign'))

request_body.setJustification('Assign Groups Admin to IT Helpdesk group')

request_body.setRoleDefinitionId('fdd7a751-b60b-444a-984c-02652fe8fa1c')

request_body.setDirectoryScopeId('/')

request_body.setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b')

scheduleInfo = RequestSchedule()
scheduleInfo.setStartDateTime(DateTime('2022-04-10T00:00:00Z'))

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.setType(ExpirationPatternType('noexpiration'))


scheduleInfo.setExpiration($scheduleInfoExpiration)

request_body.setScheduleInfo($scheduleInfo)


result = await client.roleManagement_directory_roleAssignmentScheduleRequests.post(request_body)


```