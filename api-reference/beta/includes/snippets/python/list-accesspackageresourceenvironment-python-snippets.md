---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AccessPackageResourceEnvironmentsRequestBuilder.AccessPackageResourceEnvironmentsRequestBuilderGetQueryParameters(
				filter = "originSystem eq 'SharePointOnline'",
)

request_configuration = AccessPackageResourceEnvironmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.entitlementManagement.accessPackageResourceEnvironments.get(request_configuration = request_configuration)


```