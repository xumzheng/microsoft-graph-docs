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


$transferTargetAdditionalData = [
"languageId" => 'languageId-value',
"region" => 'region-value',
];
$transferTarget->setAdditionalData($transferTargetAdditionalData);

$result =  $graphClient->communications()->callsById('call-id')->transfer()->post($requestRequestBody);


```