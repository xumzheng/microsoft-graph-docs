---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.action = 'SelfActivate'

request_body.principalId = 'c6ad1942-4afa-47f8-8d48-afb5d8d69d2f'

request_body.roleDefinitionId = '9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3'

request_body.directoryScopeId = '/'

request_body.justification = 'Need to update app roles for selected apps.'

scheduleInfo = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2021-08-17T17:40:00.000Z')

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.Type(ExpirationPatternType('afterduration'))

scheduleInfoExpiration.duration =  \DateInterval('PT5H')


scheduleInfo.expiration = scheduleInfoExpiration

request_body.scheduleInfo = scheduleInfo
ticketInfo = TicketInfo()
ticketInfo.ticketNumber = 'CONTOSO:Normal-67890'

ticketInfo.ticketSystem = 'MS Project'


request_body.ticketInfo = ticketInfo


request_configuration = RoleAssignmentScheduleRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.roleManagement.directory.roleAssignmentScheduleRequests.post(request_body = request_body)


```