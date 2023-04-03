---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CustomAccessPackageWorkflowExtension();
additionalData = [
'@odata.type' => '#microsoft.graph.customAccessPackageWorkflowExtension', 
'displayName' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
requestBody.setAdditionalData(additionalData);




graphServiceClient.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').customAccessPackageWorkflowExtensionsById('customAccessPackageWorkflowExtension-id').put(requestBody);


```