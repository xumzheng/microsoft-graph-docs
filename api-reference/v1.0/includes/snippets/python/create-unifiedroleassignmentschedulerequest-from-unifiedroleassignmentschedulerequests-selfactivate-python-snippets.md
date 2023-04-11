---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.Action(UnifiedRoleScheduleRequestActions('selfactivate'))

request_body.principalId = '071cc716-8147-4397-a5ba-b2105951cc0b'

request_body.roleDefinitionId = '8424c6f0-a189-499e-bbd0-26c1753c96d4'

request_body.directoryScopeId = '/'

request_body.justification = 'I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs'

scheduleInfo = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2022-04-14T00:00:00.000Z')

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.Type(ExpirationPatternType('afterduration'))

scheduleInfoExpiration.duration =  \DateInterval('PT5H')


scheduleInfo.expiration = scheduleInfoExpiration

request_body.scheduleInfo = scheduleInfo
ticketInfo = TicketInfo()
ticketInfo.ticketNumber = 'CONTOSO:Normal-67890'

ticketInfo.ticketSystem = 'MS Project'


request_body.ticketInfo = ticketInfo



result = await client.roleManagement.directory.roleAssignmentScheduleRequests.post(request_body = request_body)


```