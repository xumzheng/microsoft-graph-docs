---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ResumePostRequestBody()
request_body.setSource('Contoso.SodCheckProcess')

request_body.setType('microsoft.graph.accessPackageCustomExtensionStage.assignmentRequestCreated')

data = CustomExtensionData()
data.set@odatatype('microsoft.graph.accessPackageAssignmentRequestCallbackData')

additionalData = [
'stage' => 'AssignmentRequestCreated', 
'customExtensionStageInstanceId' => '857d0c50-466b-4840-bb5b-c92cea7141ff', 
'state' => 'denied', 
'customExtensionStageInstanceDetail' => 'Potential risk user based on the SOD check', 
];
data.setAdditionalData(additionalData)



request_body.setData($data)


await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequestsById('accessPackageAssignmentRequest-id').resume.post(request_body)


```