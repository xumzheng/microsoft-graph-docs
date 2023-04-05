---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.setAction('SelfActivate')

request_body.setPrincipalId('c6ad1942-4afa-47f8-8d48-afb5d8d69d2f')

request_body.setRoleDefinitionId('9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3')

request_body.setDirectoryScopeId('/')

request_body.setJustification('Need to update app roles for selected apps.')

scheduleInfo = RequestSchedule()
scheduleInfo.setStartDateTime(DateTime('2021-08-17T17:40:00.000Z'))

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.setType(ExpirationPatternType('afterduration'))

$scheduleInfoExpiration.setDuration( \DateInterval('PT5H'))


scheduleInfo.setExpiration($scheduleInfoExpiration)

request_body.setScheduleInfo($scheduleInfo)
ticketInfo = TicketInfo()
ticketInfo.setTicketNumber('CONTOSO:Normal-67890')

ticketInfo.setTicketSystem('MS Project')


request_body.setTicketInfo($ticketInfo)


result = await client.roleManagement_directory_roleAssignmentScheduleRequests.post(request_body)


```