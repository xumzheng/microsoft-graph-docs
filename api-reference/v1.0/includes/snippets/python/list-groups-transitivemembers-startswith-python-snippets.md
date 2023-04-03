---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = UserRequestBuilderGetRequestConfiguration();

query_params = UserRequestBuilderGetQueryParameters();
query_params.count = true;
query_params.orderby = ["displayName"];
query_params.filter = "startswith(displayName,%20'a')";

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.groupsById('group-id').transitiveMembers().graphUser().get(request_config);


```