---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration();

query_params = ServicePrincipalsRequestBuilderGetQueryParameters;
query_params.search = "\"displayName:Team\"";
query_params.count = true;
query_params.select = ["accountEnabled","displayName","publisherName","servicePrincipalType","signInAudience"];

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.servicePrincipals().get(request_config);


```