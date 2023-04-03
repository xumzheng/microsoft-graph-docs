---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RoleManagementPoliciesRequestBuilderGetRequestConfiguration();

queryParameters = RoleManagementPoliciesRequestBuilderGetQueryParameters();
queryParameters.filter = "scopeId eq '/' and scopeType eq 'DirectoryRole'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.policies().roleManagementPolicies().get(requestConfiguration);


```