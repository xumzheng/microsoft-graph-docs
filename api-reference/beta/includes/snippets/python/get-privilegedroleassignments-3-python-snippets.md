---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration();

queryParameters = PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters();
queryParameters.filter = "isElevated eq true and expirationDateTime eq null";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.privilegedRoleAssignments().get(requestConfiguration);


```