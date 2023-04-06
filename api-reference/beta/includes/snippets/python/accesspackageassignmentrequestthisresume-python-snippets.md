---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ResumePostRequestBody()
request_body.setSource('Contoso.SodCheckProcess')

request_body.setType('microsoft.graph.accessPackageCustomExtensionStage.assignmentRequestCreated')

data = CustomExtensionData()
data.set@odatatype('microsoft.graph.accessPackageAssignmentRequestCallbackData')

additionalData = [
'stage' => 'assignmentRequestCreated', 
'customExtensionStageInstanceId' => '957d0c50-466b-4840-bb5b-c92cea7141ff', 
'customExtensionStageInstanceDetail' => 'This user is all verified', 
];
data.setAdditionalData(additionalData)



request_body.setData($data)


await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests_by_id('accessPackageAssignmentRequest-id').resume.post(request_body, headers=)


```