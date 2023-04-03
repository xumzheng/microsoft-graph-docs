---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RoleAssignmentsRequestBuilderGetRequestConfiguration();

queryParameters = RoleAssignmentsRequestBuilderGetQueryParameters();
queryParameters.filter = "principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.roleManagement().deviceManagement().roleAssignments().get(requestConfiguration);


```