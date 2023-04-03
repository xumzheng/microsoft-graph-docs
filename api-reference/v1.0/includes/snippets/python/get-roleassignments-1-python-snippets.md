---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RoleAssignmentsRequestBuilderGetRequestConfiguration();

queryParameters = RoleAssignmentsRequestBuilderGetQueryParameters();
queryParameters.filter = "roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'";
queryParameters.expand = ["principal"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.roleManagement().directory().roleAssignments().get(requestConfiguration);


```