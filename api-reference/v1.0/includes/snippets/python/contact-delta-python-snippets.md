---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = DeltaRequestBuilderGetRequestConfiguration();

query_params = DeltaRequestBuilderGetQueryParameters();
query_params.select = ["displayName"];

headers = [
'Prefer' => 'odata.maxpagesize=2',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.me().contactFoldersById('contactFolder-id').contacts().delta().get(request_config);


```