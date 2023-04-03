---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = UsersRequestBuilderGetRequestConfiguration();

query_params = UsersRequestBuilderGetQueryParameters();
query_params.search = "\"displayName:wa\" OR \"displayName:ad\"";
query_params.orderby = ["displayName"];
query_params.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.users().get(request_config);


```