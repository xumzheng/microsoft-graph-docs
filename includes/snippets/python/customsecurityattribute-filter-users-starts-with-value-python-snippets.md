---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = UsersRequestBuilderGetRequestConfiguration();

query_params = UsersRequestBuilderGetQueryParameters();
query_params.count = true;
query_params.select = ["id","displayName","customSecurityAttributes"];
query_params.filter = "startsWith(customSecurityAttributes/Marketing/EmployeeId,'GS')";

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.users().get(request_config);


```