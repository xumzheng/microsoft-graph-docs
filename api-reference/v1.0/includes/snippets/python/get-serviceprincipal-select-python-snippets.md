---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ServicePrincipalRequestBuilderGetRequestConfiguration();

query_params = ServicePrincipalRequestBuilderGetQueryParameters();
query_params.select = ["id","appId","displayName","appRoles","oauth2PermissionScopes"];

request_config.queryParameters = query_params;


result = awaitclient.servicePrincipalsById('servicePrincipal-id').get(request_config);


```