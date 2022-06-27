---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TransferPostRequestBody();



$transferTarget = new InvitationParticipantInfo();
$requestRequestBody->setTransferTarget($transferTarget);



$identity = new IdentitySet();
$transferTarget->setIdentity($identity);



$user = new Identity();
$identity->setUser($user);


$user->setId('550fae72-d251-43ec-868c-373732c2704f');
$user->setDisplayName('Heidi Steen');
$userAdditionalData = [
	"@odata.type" => '#microsoft.graph.identity',
];
$user->setAdditionalData($userAdditionalData);

$identityAdditionalData = [
"@odata.type" => '#microsoft.graph.identitySet',
];
$identity->setAdditionalData($identityAdditionalData);

$transferTarget->setReplacesCallId('e5d39592-99bd-4db8-bca8-30fb894ec51d');
$transferTargetAdditionalData = [
"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
"endpointType" => 'default',
];
$transferTarget->setAdditionalData($transferTargetAdditionalData);

$result =  $graphClient->communications()->callsById('call-id')->transfer()->post($requestRequestBody);


```