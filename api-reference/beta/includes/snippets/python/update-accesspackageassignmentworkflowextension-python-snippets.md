---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageCustomWorkflowExtension()
additionalData = [
'@odata.type' => '#microsoft.graph.accessPackageAssignmentWorkflowExtension', 
'displayName' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
request_body.setAdditionalData(additionalData)




await client.identityGovernance.entitlementManagement.accessPackageCatalogsby_id('accessPackageCatalog-id').accessPackageCustomWorkflowExtensionsby_id('customCalloutExtension-id').put(request_body)


```