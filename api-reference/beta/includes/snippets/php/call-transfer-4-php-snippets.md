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


$identityAdditionalData = [
	"@odata.type" => '#microsoft.graph.identitySet',
];
$identity->setAdditionalData($identityAdditionalData);

$transferTarget->setReplacesCallId('e5d39592-99bd-4db8-bca8-30fb894ec51d');
$transferTargetAdditionalData = [
"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
"languageId" => 'en-us',
"region" => 'amer',
];
$transferTarget->setAdditionalData($transferTargetAdditionalData);

$result =  $graphClient->communications()->callsById('call-id')->transfer()->post($requestRequestBody);


```