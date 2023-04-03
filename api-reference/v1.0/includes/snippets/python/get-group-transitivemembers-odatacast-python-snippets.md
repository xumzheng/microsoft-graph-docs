---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = GroupRequestBuilderGetRequestConfiguration();

query_params = GroupRequestBuilderGetQueryParameters();
query_params.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.groupsById('group-id').transitiveMembers().graphGroup().get(request_config);


```