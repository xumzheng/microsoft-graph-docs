---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = GroupsRequestBuilderGetRequestConfiguration();

query_params = GroupsRequestBuilderGetQueryParameters();
query_params.search = "\"displayName:Video\" OR \"description:prod\"";
query_params.orderby = ["displayName"];
query_params.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.groups().get(request_config);


```