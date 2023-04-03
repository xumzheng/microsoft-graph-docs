---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UnifiedRoleAssignment();
requestBody.set@odatatype('#microsoft.graph.unifiedRoleAssignment');

requestBody.setRoleDefinitionId('c2cf284d-6c41-4e6b-afac-4b80928c9034');

requestBody.setPrincipalId('f8ca5a85-489a-49a0-b555-0a6d81e56f0d');

requestBody.setDirectoryScopeId('/');



result = awaitclient.roleManagement().directory().roleAssignments().post(requestBody);


```