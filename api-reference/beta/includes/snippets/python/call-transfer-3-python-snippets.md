---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TransferPostRequestBody();
$transferTarget = new InvitationParticipantInfo();
$transferTarget.setEndpointType(new EndpointType('default'));

$transferTargetIdentity = new IdentitySet();
$additionalData = [
'phone' => $transferTargetIdentity = new Phone();
$		transferTargetIdentity.set@odatatype('#microsoft.graph.identity');

$		transferTargetIdentity.setId('+12345678901');


$transferTargetIdentity.setPhone($phone);

];
$transferTargetIdentity.setAdditionalData($additionalData);



$transferTarget.setIdentity($transferTargetIdentity);
$additionalData = [
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
$transferTarget.setAdditionalData($additionalData);



$requestBody.setTransferTarget($transferTarget);


$graphServiceClient.communications().callsById('call-id').transfer().post($requestBody);


```