---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UnifiedRoleEligibilityScheduleRequest();
requestBody.setAction(UnifiedRoleScheduleRequestActions('adminassign'));

requestBody.setJustification('Assign User Admin eligibility to IT Helpdesk (User) group');

requestBody.setRoleDefinitionId('fe930be7-5e62-47db-91af-98c3a49a38b1');

requestBody.setDirectoryScopeId('/');

requestBody.setPrincipalId('e77cbb23-0ff2-4e18-819c-690f58269752');

scheduleInfo = RequestSchedule();
scheduleInfo.setStartDateTime(DateTime('2021-07-01T00:00:00Z'));

scheduleInfoExpiration = ExpirationPattern();
scheduleInfoExpiration.setEndDateTime(DateTime('2022-06-30T00:00:00Z'));

scheduleInfoExpiration.setType(ExpirationPatternType('afterdatetime'));


scheduleInfo.setExpiration($scheduleInfoExpiration);

requestBody.setScheduleInfo($scheduleInfo);


result = awaitclient.roleManagement().directory().roleEligibilityScheduleRequests().post(requestBody);


```