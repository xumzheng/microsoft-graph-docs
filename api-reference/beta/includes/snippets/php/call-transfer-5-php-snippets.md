---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TransferPostRequestBody();



$transferTarget = new InvitationParticipantInfo();
$requestRequestBody->setTransferTarget($transferTarget);


$transferTarget->setEndpointType(new EndpointType('default'));

$identity = new IdentitySet();
$transferTarget->setIdentity($identity);



$user = new Identity();
$identity->setUser($user);


$user->setId('550fae72-d251-43ec-868c-373732c2704f');
$user->setDisplayName('Heidi Steen');
$userAdditionalData = [
	"tenantId" => '72f988bf-86f1-41af-91ab-2d7cd011db47',
];
$user->setAdditionalData($userAdditionalData);




$transferee = new ParticipantInfo();
$requestRequestBody->setTransferee($transferee);



$identity = new IdentitySet();
$transferee->setIdentity($identity);



$user = new Identity();
$identity->setUser($user);


$user->setId('751f6800-3180-414d-bd94-333364659951');
$userAdditionalData = [
"tenantId" => '72f988bf-86f1-41af-91ab-2d7cd011db47',
];
$user->setAdditionalData($userAdditionalData);


$transferee->setParticipantId('909c6581-5130-43e9-88f3-fcb3582cde37');

$requestRequestBodyAdditionalData = [
"languageId" => 'languageId-value',
"region" => 'region-value',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->communications()->callsById('call-id')->transfer()->post($requestRequestBody);


```