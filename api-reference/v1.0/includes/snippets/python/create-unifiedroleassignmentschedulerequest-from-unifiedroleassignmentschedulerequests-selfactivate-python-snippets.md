---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentScheduleRequest()
request_body.setAction(UnifiedRoleScheduleRequestActions('selfactivate'))

request_body.setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b')

request_body.setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4')

request_body.setDirectoryScopeId('/')

request_body.setJustification('I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs')

scheduleInfo = RequestSchedule()
scheduleInfo.setStartDateTime(DateTime('2022-04-14T00:00:00.000Z'))

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