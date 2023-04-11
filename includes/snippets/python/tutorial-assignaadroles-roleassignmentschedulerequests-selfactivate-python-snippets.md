---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.Action(UnifiedRoleScheduleRequestActions('selfactivate'))

request_body.principalId = '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'

request_body.roleDefinitionId = 'fe930be7-5e62-47db-91af-98c3a49a38b1'

request_body.directoryScopeId = '/'

request_body.justification = 'Need to invalidate all app refresh tokens for Contoso users.'

scheduleInfo = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2021-09-04T15:13:00.000Z')

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.Type(ExpirationPatternType('afterduration'))

scheduleInfoExpiration.duration =  \DateInterval('PT5H')


scheduleInfo.expiration = scheduleInfoExpiration

request_body.scheduleInfo = scheduleInfo
ticketInfo = TicketInfo()
ticketInfo.ticketNumber = 'CONTOSO:Security-012345'

ticketInfo.ticketSystem = 'Contoso ICM'


request_body.ticketInfo = ticketInfo


request_configuration = RoleAssignmentScheduleRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.roleManagement.directory.roleAssignmentScheduleRequests.post(request_body = request_body)


```