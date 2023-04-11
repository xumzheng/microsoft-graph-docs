---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = IncompatibleAccessPackagesRequestBuilderGetRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').incompatibleAccessPackages.get()


```