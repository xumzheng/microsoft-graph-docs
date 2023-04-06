---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackage()
request_body.setCatalogId('aa2f6514-3232-46e7-a08a-2411ad8d7128')

request_body.setDisplayName('sales reps')

request_body.setDescription('outside sales representatives')


request_config = AccessPackagesRequestBuilderPostRequestConfiguration(
request_config = AccessPackagesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.accessPackages.post(request_body, headers=)


```