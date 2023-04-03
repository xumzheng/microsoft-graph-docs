---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration();

queryParameters = UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters();
queryParameters.expand = ["roleDefinition"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.roleManagement().cloudPC().roleAssignmentsById('unifiedRoleAssignmentMultiple-id').get(requestConfiguration);


```