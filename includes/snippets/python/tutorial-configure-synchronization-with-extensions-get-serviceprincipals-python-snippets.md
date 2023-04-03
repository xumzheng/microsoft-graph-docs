---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration();

query_params = ServicePrincipalsRequestBuilderGetQueryParameters();
query_params.select = ["id","appId","displayName"];
query_params.filter = "startswith(displayName,%20'salesforce')";

headers = [
'Authorization' => 'Bearer {Token}',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.servicePrincipals().get(request_config);


```