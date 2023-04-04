---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UnifiedRoleEligibilityScheduleRequest();
request_body.setAction(UnifiedRoleScheduleRequestActions('adminassign'));

request_body.setJustification('Assign Attribute Assignment Admin eligibility to restricted user');

request_body.setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4');

request_body.setDirectoryScopeId('/');

request_body.setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');

scheduleInfo = RequestSchedule();
scheduleInfo.setStartDateTime(DateTime('2022-04-10T00:00:00Z'));

scheduleInfoExpiration = ExpirationPattern();
scheduleInfoExpiration.setType(ExpirationPatternType('afterdatetime'));

scheduleInfoExpiration.setEndDateTime(DateTime('2024-04-10T00:00:00Z'));


scheduleInfo.setExpiration($scheduleInfoExpiration);

request_body.setScheduleInfo($scheduleInfo);


result = await client.roleManagement().directory().roleEligibilityScheduleRequests().post(request_body);


```