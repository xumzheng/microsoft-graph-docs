---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RoleAssignmentsRequestBuilderGetRequestConfiguration();

queryParameters = RoleAssignmentsRequestBuilderGetQueryParameters();
queryParameters.filter = "appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'";
queryParameters.expand = ["principal"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.roleManagement().entitlementManagement().roleAssignments().get(requestConfiguration);


```