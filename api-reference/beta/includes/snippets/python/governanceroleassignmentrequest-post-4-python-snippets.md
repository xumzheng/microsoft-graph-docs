---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GovernanceRoleAssignmentRequest();
request_body.setRoleDefinitionId('65bb4622-61f5-4f25-9d75-d0e20cf92019');

request_body.setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5');

request_body.setSubjectId('74765671-9ca4-40d7-9e36-2f4a570608a6');

request_body.setAssignmentState('Eligible');

request_body.setType('AdminRemove');



result = await client.privilegedAccessById('privilegedAccess-id').roleAssignmentRequests().post(request_body);


```