---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageCustomWorkflowExtension();
additionalData = [
'@odata.type' => '#microsoft.graph.accessPackageAssignmentWorkflowExtension', 
'displayName' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').accessPackageCustomWorkflowExtensionsById('customCalloutExtension-id').put(requestBody);


```