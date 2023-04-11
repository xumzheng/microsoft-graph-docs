---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.action = 'AdminRemove'

request_body.justification = 'Assign User Admin eligibility to IT Helpdesk (User) group'

request_body.roleDefinitionId = 'fdd7a751-b60b-444a-984c-02652fe8fa1c'

request_body.directoryScopeId = '/'

request_body.principalId = '07706ff1-46c7-4847-ae33-3003830675a1'

scheduleInfo = RequestSchedule()
scheduleInfo.startDateTime = DateTime('2021-07-26T18:08:06.2081758Z')

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.endDateTime = DateTime('2022-06-30T00:00:00Z')

scheduleInfoExpiration.Type(ExpirationPatternType('afterdatetime'))


scheduleInfo.expiration = scheduleInfoExpiration

request_body.scheduleInfo = scheduleInfo



result = await client.roleManagement.directory.roleEligibilityScheduleRequests.post(request_body = request_body)


```