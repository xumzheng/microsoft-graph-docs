---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageCustomWorkflowExtension()
additionalData = [
'@odata.type' => '#microsoft.graph.accessPackageAssignmentRequestWorkflowExtension', 
'displayName' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
request_body.setAdditionalData(additionalData)




await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageCustomWorkflowExtensions_by_id('customCalloutExtension-id').put(request_body, headers=)


```