---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RoleAssignmentsRequestBuilderGetRequestConfiguration();

queryParameters = RoleAssignmentsRequestBuilderGetQueryParameters();
queryParameters.filter = " principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.roleManagement().directory().roleAssignments().get(requestConfiguration);


```