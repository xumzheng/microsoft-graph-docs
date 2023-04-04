---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TransferPostRequestBody();
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



request_body.setTransferTarget($transferTarget);
additionalData = [
'clientContext' => '9e90d1c1-f61e-43e7-9f75-d420159aae08', 
];
request_body.setAdditionalData(additionalData);




await client.communications.callsById('call-id').transfer.post(request_body);


```