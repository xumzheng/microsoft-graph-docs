---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomAccessPackageWorkflowExtension()
additionalData = [
'@odata.type' => '#microsoft.graph.customAccessPackageWorkflowExtension', 
'displayName' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
request_body.setAdditionalData(additionalData)




await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').customAccessPackageWorkflowExtensions_by_id('customAccessPackageWorkflowExtension-id').put(request_body)


```