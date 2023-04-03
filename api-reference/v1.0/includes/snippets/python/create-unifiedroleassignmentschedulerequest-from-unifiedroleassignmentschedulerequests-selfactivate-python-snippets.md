---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedRoleAssignmentScheduleRequest();
requestBody.setAction(UnifiedRoleScheduleRequestActions('selfactivate'));

requestBody.setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');

requestBody.setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4');

requestBody.setDirectoryScopeId('/');

requestBody.setJustification('I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs');

scheduleInfo = RequestSchedule();
scheduleInfo.setStartDateTime(DateTime('2022-04-14T00:00:00.000Z'));

scheduleInfoExpiration = ExpirationPattern();
scheduleInfoExpiration.setType(ExpirationPatternType('afterduration'));

$scheduleInfoExpiration.setDuration( \DateInterval('PT5H'));


scheduleInfo.setExpiration($scheduleInfoExpiration);

requestBody.setScheduleInfo($scheduleInfo);
ticketInfo = TicketInfo();
ticketInfo.setTicketNumber('CONTOSO:Normal-67890');

ticketInfo.setTicketSystem('MS Project');


requestBody.setTicketInfo($ticketInfo);


result = await client.roleManagement().directory().roleAssignmentScheduleRequests().post(requestBody);


```