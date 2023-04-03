---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UnifiedRoleAssignmentRequestBuilderGetRequestConfiguration();

queryParameters = UnifiedRoleAssignmentRequestBuilderGetQueryParameters();
queryParameters.expand = ["roleDefinition"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.roleManagement().directory().roleAssignmentsById('unifiedRoleAssignment-id').get(requestConfiguration);


```