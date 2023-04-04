---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = UnifiedRoleAssignmentRequestBuilderGetRequestConfiguration();

query_params = UnifiedRoleAssignmentRequestBuilderGetQueryParameters;
query_params.expand = ["roleDefinition"];

request_config.queryParameters = query_params;


result = await client.roleManagement().directory().roleAssignmentsById('unifiedRoleAssignment-id').get(request_config);


```