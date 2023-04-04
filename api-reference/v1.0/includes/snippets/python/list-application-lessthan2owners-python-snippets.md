---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = ApplicationsRequestBuilderGetRequestConfiguration();

query_params = ApplicationsRequestBuilderGetQueryParameters();
query_params.filter = "owners/$count eq 0 or owners/$count eq 1";
query_params.count = true;
query_params.select = ["id","displayName"];

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.applications.get(request_config);


```