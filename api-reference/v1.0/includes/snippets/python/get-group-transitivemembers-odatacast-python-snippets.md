---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = GroupRequestBuilderGetRequestConfiguration();

query_params = GroupRequestBuilderGetQueryParameters();
query_params.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.groupsById('group-id').transitiveMembers().graphGroup().get(request_config);


```