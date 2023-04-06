---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.setAction('AdminAssign')

request_body.setJustification('Assign User Admin eligibility to IT Helpdesk (User) group')

request_body.setRoleDefinitionId('fdd7a751-b60b-444a-984c-02652fe8fa1c')

request_body.setDirectoryScopeId('/')

request_body.setPrincipalId('07706ff1-46c7-4847-ae33-3003830675a1')

scheduleInfo = RequestSchedule()
scheduleInfo.setStartDateTime(DateTime('2021-07-01T00:00:00Z'))

scheduleInfoExpiration = ExpirationPattern()
scheduleInfoExpiration.setEndDateTime(DateTime('2022-06-30T00:00:00Z'))

scheduleInfoExpiration.setType(ExpirationPatternType('afterdatetime'))


scheduleInfo.setExpiration($scheduleInfoExpiration)

request_body.setScheduleInfo($scheduleInfo)

request_config = RoleEligibilityScheduleRequestsRequestBuilderPostRequestConfiguration(
request_config = RoleEligibilityScheduleRequestsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.roleManagement.directory.roleEligibilityScheduleRequests.post(request_body, headers=)


```