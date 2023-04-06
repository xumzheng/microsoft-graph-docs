---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.setAction(UnifiedRoleScheduleRequestActions('selfactivate'))

request_body.setPrincipalId('7146daa8-1b4b-4a66-b2f7-cf593d03c8d2')

request_body.setRoleDefinitionId('fe930be7-5e62-47db-91af-98c3a49a38b1')

request_body.setDirectoryScopeId('/')

request_body.setJustification('Need to invalidate all app refresh tokens for Contoso users.')

scheduleInfo = RequestSchedule()
scheduleInfo.setStartDateTime(DateTime('2021-09-04T15:13:00.000Z'))

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.setType(ExpirationPatternType('afterduration'))

$scheduleInfoExpiration.setDuration( \DateInterval('PT5H'))


scheduleInfo.setExpiration($scheduleInfoExpiration)

request_body.setScheduleInfo($scheduleInfo)
ticketInfo = TicketInfo()
ticketInfo.setTicketNumber('CONTOSO:Security-012345')

ticketInfo.setTicketSystem('Contoso ICM')


request_body.setTicketInfo($ticketInfo)


result = await client.roleManagement.directory.roleAssignmentScheduleRequests.post(request_body, headers=)


```