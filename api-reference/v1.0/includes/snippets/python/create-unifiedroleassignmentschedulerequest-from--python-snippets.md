---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UnifiedRoleAssignmentScheduleRequest();
requestBody.setAction(UnifiedRoleScheduleRequestActions('adminassign'));

requestBody.setJustification('Assign Groups Admin to IT Helpdesk group');

requestBody.setRoleDefinitionId('fdd7a751-b60b-444a-984c-02652fe8fa1c');

requestBody.setDirectoryScopeId('/');

requestBody.setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');

scheduleInfo = RequestSchedule();
scheduleInfo.setStartDateTime(DateTime('2022-04-10T00:00:00Z'));

scheduleInfoExpiration = ExpirationPattern();
scheduleInfoExpiration.setType(ExpirationPatternType('noexpiration'));


scheduleInfo.setExpiration($scheduleInfoExpiration);

requestBody.setScheduleInfo($scheduleInfo);


result = awaitclient.roleManagement().directory().roleAssignmentScheduleRequests().post(requestBody);


```