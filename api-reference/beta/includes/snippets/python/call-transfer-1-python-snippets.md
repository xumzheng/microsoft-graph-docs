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
transferTargetIdentityUser = Identity();
transferTargetIdentityUser.setId('550fae72-d251-43ec-868c-373732c2704f');

transferTargetIdentityUser.setDisplayName('Heidi Steen');

additionalData = [
'tenantId' => '72f988bf-86f1-41af-91ab-2d7cd011db47', 
];
transferTargetIdentityUser.setAdditionalData(additionalData);



transferTargetIdentity.setUser($transferTargetIdentityUser);

transferTarget.setIdentity($transferTargetIdentity);
additionalData = [
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
transferTarget.setAdditionalData(additionalData);



requestBody.setTransferTarget($transferTarget);


graphServiceClient.communications().callsById('call-id').transfer().post(requestBody);


```