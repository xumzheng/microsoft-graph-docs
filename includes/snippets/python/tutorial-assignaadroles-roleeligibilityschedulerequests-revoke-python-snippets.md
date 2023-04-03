---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedRoleEligibilityScheduleRequest();
requestBody.setAction(UnifiedRoleScheduleRequestActions('adminremove'));

requestBody.setPrincipalId('e77cbb23-0ff2-4e18-819c-690f58269752');

requestBody.setRoleDefinitionId('fe930be7-5e62-47db-91af-98c3a49a38b1');

requestBody.setDirectoryScopeId('/');



result = await client.roleManagement().directory().roleEligibilityScheduleRequests().post(requestBody);


```