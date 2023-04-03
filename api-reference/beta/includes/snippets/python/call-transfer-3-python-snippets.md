---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TransferPostRequestBody();
transferTarget = InvitationParticipantInfo();
transferTarget.setEndpointType(EndpointType('default'));

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
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
transferTarget.setAdditionalData(additionalData);



requestBody.setTransferTarget($transferTarget);


graphServiceClient.communications().callsById('call-id').transfer().post(requestBody);


```