---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AppRoleAssignedResourcesRequestBuilderGetRequestConfiguration();

queryParameters = AppRoleAssignedResourcesRequestBuilderGetQueryParameters();
queryParameters.select = ["displayName","accountEnabled","servicePrincipalType","signInAudience"];

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().appRoleAssignedResources().get(requestConfiguration);


```