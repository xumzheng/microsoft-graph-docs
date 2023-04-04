---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AccessPackageCatalogsRequestBuilderGetRequestConfiguration();

query_params = AccessPackageCatalogsRequestBuilderGetQueryParameters();
query_params.filter = "(displayName eq 'General')";

request_config.queryParameters = query_params;


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs.get(request_config);


```