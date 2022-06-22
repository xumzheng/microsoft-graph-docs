---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Call();


$requestRequestBody->setCallbackUri('https://bot.contoso.com/callback');

$source = new ParticipantInfo();
$requestRequestBody->setSource($source);



$identity = new IdentitySet();
$source->setIdentity($identity);


$identityAdditionalData = [
	"@odata.type" => '#microsoft.graph.identitySet',
];
$identity->setAdditionalData($identityAdditionalData);

$source->setCountryCode(null);
$source->setEndpointType(null);
$source->setRegion(null);
$source->setLanguageId(null);
$sourceAdditionalData = [
"@odata.type" => '#microsoft.graph.participantInfo',
];
$source->setAdditionalData($sourceAdditionalData);

$targetsArray = [];

$targets1 = new InvitationParticipantInfo();


$identity = new IdentitySet();
$targets1->setIdentity($identity);


$identityAdditionalData = [
"@odata.type" => '#microsoft.graph.identitySet',
];
$identity->setAdditionalData($identityAdditionalData);

$targets1AdditionalData = [
"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
];
$targets1->setAdditionalData($targets1AdditionalData);

$targetsArray []= $targets1;
$requestRequestBody->setTargets($targetsArray);
$requestedModalitiesArray = [];
'audio',$requestedModalitiesArray []= $requestedModalities1;
$requestRequestBody->setRequestedModalities($requestedModalitiesArray);

$mediaConfig = new MediaConfig();
$requestRequestBody->setMediaConfig($mediaConfig);


$mediaConfigAdditionalData = [
"@odata.type" => '#microsoft.graph.serviceHostedMediaConfig',
];
$mediaConfig->setAdditionalData($mediaConfigAdditionalData);

$requestRequestBody->setTenantId('aa67bd4c-8475-432d-bd41-39f255720e0a');
$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.call',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->communications()->calls()->post($requestRequestBody);


```