---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TransferPostRequestBody();
transferTarget = InvitationParticipantInfo();
transferTargetIdentity = IdentitySet();
additionalData = [
'phone' => transferTargetIdentity = Phone();
		transferTargetIdentity.set@odatatype('#microsoft.graph.identity');

		transferTargetIdentity.setId('+12345678901');


transferTargetIdentity.setPhone($phone);

];
transferTargetIdentity.setAdditionalData(additionalData);



transferTarget.setIdentity($transferTargetIdentity);
additionalData = [
'endpointType' => 'default', 
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
transferTarget.setAdditionalData(additionalData);



requestBody.setTransferTarget($transferTarget);
additionalData = [
'clientContext' => '9e90d1c1-f61e-43e7-9f75-d420159aae08', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.communications().callsById('call-id').transfer().post(requestBody);


```