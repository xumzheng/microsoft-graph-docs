---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = CustomAccessPackageWorkflowExtensionRequestBuilderGetRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').customAccessPackageWorkflowExtensions_by_id('customAccessPackageWorkflowExtension-id').get()


```