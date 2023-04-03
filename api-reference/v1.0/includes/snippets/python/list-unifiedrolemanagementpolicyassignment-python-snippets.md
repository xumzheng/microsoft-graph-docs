---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration();

queryParameters = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters();
queryParameters.filter = "scopeId eq '/' and scopeType eq 'Directory'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.policies().roleManagementPolicyAssignments().get(requestConfiguration);


```