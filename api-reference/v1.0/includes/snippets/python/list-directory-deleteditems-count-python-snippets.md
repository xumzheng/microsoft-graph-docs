---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = GroupRequestBuilderGetRequestConfiguration();

query_params = GroupRequestBuilderGetQueryParameters();
query_params.count = true;
query_params.orderby = ["deletedDateTime asc"];
query_params.select = ["id","DisplayName","deletedDateTime"];

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.directory.deletedItems.graphgroup.get(request_config);


```