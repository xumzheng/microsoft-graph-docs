---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackage()
request_body.displayName = 'Access Package New Name'



request_configuration = AccessPackageRequestBuilderPatchRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').patch(request_body = request_body)


```