---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CustomAccessPackageWorkflowExtension();
additionalData = [
'@odata.type' => '#microsoft.graph.customAccessPackageWorkflowExtension', 
'displayName' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
requestBody.setAdditionalData(additionalData);




await client.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').customAccessPackageWorkflowExtensionsById('customAccessPackageWorkflowExtension-id').put(requestBody);


```