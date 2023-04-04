---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration();

query_params = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters;
query_params.filter = "scopeId eq '/' and scopeType eq 'DirectoryRole' and roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'";
query_params.expand = ["policy($expand=rules)"];

request_config.queryParameters = query_params;


result = await client.policies().roleManagementPolicyAssignments().get(request_config);


```