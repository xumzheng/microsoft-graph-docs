---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration();

query_params = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters();
query_params.filter = "scopeId eq '/' and scopeType eq 'Directory'";

request_config.queryParameters = query_params;


result = awaitclient.policies().roleManagementPolicyAssignments().get(request_config);


```