---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TransferPostRequestBody();
transferTarget = InvitationParticipantInfo();
transferTarget.setEndpointType(EndpointType('default'));

transferTargetIdentity = IdentitySet();
transferTargetIdentityUser = Identity();
transferTargetIdentityUser.setId('550fae72-d251-43ec-868c-373732c2704f');

transferTargetIdentityUser.setDisplayName('Heidi Steen');

additionalData = [
'tenantId' => '72f988bf-86f1-41af-91ab-2d7cd011db47', 
];
transferTargetIdentityUser.setAdditionalData(additionalData);



transferTargetIdentity.setUser($transferTargetIdentityUser);

transferTarget.setIdentity($transferTargetIdentity);

request_body.setTransferTarget($transferTarget);
transferee = ParticipantInfo();
transfereeIdentity = IdentitySet();
transfereeIdentityUser = Identity();
transfereeIdentityUser.setId('751f6800-3180-414d-bd94-333364659951');

additionalData = [
'tenantId' => '72f988bf-86f1-41af-91ab-2d7cd011db47', 
];
transfereeIdentityUser.setAdditionalData(additionalData);



transfereeIdentity.setUser($transfereeIdentityUser);

transferee.setIdentity($transfereeIdentity);
transferee.setParticipantId('909c6581-5130-43e9-88f3-fcb3582cde37');


request_body.setTransferee($transferee);
additionalData = [
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
request_body.setAdditionalData(additionalData);




await client.communications.callsById('call-id').transfer.post(request_body);


```