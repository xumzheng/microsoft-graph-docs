---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = AppRoleAssignedResourcesRequestBuilderGetRequestConfiguration();

query_params = AppRoleAssignedResourcesRequestBuilderGetQueryParameters();
query_params.select = ["displayName","accountEnabled","servicePrincipalType","signInAudience"];

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.me().appRoleAssignedResources().get(request_config);


```