---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration();

query_params = ServicePrincipalsRequestBuilderGetQueryParameters();
query_params.filter = "displayName eq 'Microsoft Graph'";
query_params.select = ["id","displayName","appId","appRoles"];

request_config.queryParameters = query_params;


result = awaitclient.servicePrincipals().get(request_config);


```