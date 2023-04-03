---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ApplicationsRequestBuilderGetRequestConfiguration();

query_params = ApplicationsRequestBuilderGetQueryParameters();
query_params.search = "\"displayName:Web\"";
query_params.count = true;
query_params.select = ["appId","identifierUris","displayName","publisherDomain","signInAudience"];

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.applications().get(request_config);


```