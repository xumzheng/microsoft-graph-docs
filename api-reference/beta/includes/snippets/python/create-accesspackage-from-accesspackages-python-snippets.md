---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackage()
request_body.catalogId = 'aa2f6514-3232-46e7-a08a-2411ad8d7128'

request_body.displayName = 'sales reps'

request_body.description = 'outside sales representatives'



request_configuration = AccessPackagesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackages.post(request_body = request_body)


```