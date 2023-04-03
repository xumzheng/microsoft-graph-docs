---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PartnersRequestBuilderGetRequestConfiguration();

query_params = PartnersRequestBuilderGetQueryParameters();
query_params.select = ["tenantId"];
query_params.expand = ["identitySynchronization"];

request_config.queryParameters = query_params;


result = awaitclient.policies().crossTenantAccessPolicy().partners().get(request_config);


```