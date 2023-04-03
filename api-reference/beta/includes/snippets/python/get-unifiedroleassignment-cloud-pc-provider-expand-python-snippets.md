---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration();

query_params = UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters();
query_params.expand = ["roleDefinition"];

request_config.queryParameters = query_params;


result = awaitclient.roleManagement().cloudPC().roleAssignmentsById('unifiedRoleAssignmentMultiple-id').get(request_config);


```