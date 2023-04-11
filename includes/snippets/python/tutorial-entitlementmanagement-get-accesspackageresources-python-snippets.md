---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AccessPackageResourcesRequestBuilder.AccessPackageResourcesRequestBuilderGetQueryParameters(
				filter = "(displayName eq 'Marketing resources')",
)

request_configuration = AccessPackageResourcesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageResources.get(request_configuration = request_configuration)


```