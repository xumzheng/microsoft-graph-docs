---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedRoleEligibilityScheduleRequest();
requestBody.setAction(UnifiedRoleScheduleRequestActions('adminassign'));

requestBody.setJustification('Assign Attribute Assignment Admin eligibility to restricted user');

requestBody.setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4');

requestBody.setDirectoryScopeId('/');

requestBody.setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');

scheduleInfo = RequestSchedule();
scheduleInfo.setStartDateTime(DateTime('2022-04-10T00:00:00Z'));

scheduleInfoExpiration = ExpirationPattern();
scheduleInfoExpiration.setType(ExpirationPatternType('afterdatetime'));

scheduleInfoExpiration.setEndDateTime(DateTime('2024-04-10T00:00:00Z'));


scheduleInfo.setExpiration($scheduleInfoExpiration);

requestBody.setScheduleInfo($scheduleInfo);


result = await client.roleManagement().directory().roleEligibilityScheduleRequests().post(requestBody);


```