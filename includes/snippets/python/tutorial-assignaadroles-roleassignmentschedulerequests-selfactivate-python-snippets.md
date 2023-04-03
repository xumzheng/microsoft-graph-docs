---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UnifiedRoleAssignmentScheduleRequest();
requestBody.setAction(UnifiedRoleScheduleRequestActions('selfactivate'));

requestBody.setPrincipalId('7146daa8-1b4b-4a66-b2f7-cf593d03c8d2');

requestBody.setRoleDefinitionId('fe930be7-5e62-47db-91af-98c3a49a38b1');

requestBody.setDirectoryScopeId('/');

requestBody.setJustification('Need to invalidate all app refresh tokens for Contoso users.');

scheduleInfo = RequestSchedule();
scheduleInfo.setStartDateTime(DateTime('2021-09-04T15:13:00.000Z'));

scheduleInfoExpiration = ExpirationPattern();
scheduleInfoExpiration.setType(ExpirationPatternType('afterduration'));

$scheduleInfoExpiration.setDuration( \DateInterval('PT5H'));


scheduleInfo.setExpiration($scheduleInfoExpiration);

requestBody.setScheduleInfo($scheduleInfo);
ticketInfo = TicketInfo();
ticketInfo.setTicketNumber('CONTOSO:Security-012345');

ticketInfo.setTicketSystem('Contoso ICM');


requestBody.setTicketInfo($ticketInfo);


requestResult = graphServiceClient.roleManagement().directory().roleAssignmentScheduleRequests().post(requestBody);


```