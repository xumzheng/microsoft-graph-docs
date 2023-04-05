---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageResourceEnvironmentsRequestBuilderGetRequestConfiguration(
query_params = AccessPackageResourceEnvironmentsRequestBuilderGetQueryParameters()
query_params.filter = "originSystem eq 'SharePointOnline'"

)


result = await client.identityGovernance.entitlementManagement.accessPackageResourceEnvironments.get(request_config)


```