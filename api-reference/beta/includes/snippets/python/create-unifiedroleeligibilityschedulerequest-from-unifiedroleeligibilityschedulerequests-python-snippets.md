---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedRoleEligibilityScheduleRequest();
requestBody.setAction('AdminAssign');

requestBody.setJustification('Assign User Admin eligibility to IT Helpdesk (User) group');

requestBody.setRoleDefinitionId('fdd7a751-b60b-444a-984c-02652fe8fa1c');

requestBody.setDirectoryScopeId('/');

requestBody.setPrincipalId('07706ff1-46c7-4847-ae33-3003830675a1');

scheduleInfo = RequestSchedule();
scheduleInfo.setStartDateTime(DateTime('2021-07-01T00:00:00Z'));

scheduleInfoExpiration = ExpirationPattern();
scheduleInfoExpiration.setEndDateTime(DateTime('2022-06-30T00:00:00Z'));

scheduleInfoExpiration.setType(ExpirationPatternType('afterdatetime'));


scheduleInfo.setExpiration($scheduleInfoExpiration);

requestBody.setScheduleInfo($scheduleInfo);


result = await client.roleManagement().directory().roleEligibilityScheduleRequests().post(requestBody);


```