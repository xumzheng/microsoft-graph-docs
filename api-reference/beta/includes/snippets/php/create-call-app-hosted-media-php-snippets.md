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



$application = new Identity();
$identity->setApplication($application);


$application->setDisplayName('Calling Bot');
$application->setId('2891555a-92ff-42e6-80fa-6e1300c6b5c6');
$applicationAdditionalData = [
	"@odata.type" => '#microsoft.graph.identity',
];
$application->setAdditionalData($applicationAdditionalData);

$identityAdditionalData = [
"@odata.type" => '#microsoft.graph.identitySet',
];
$identity->setAdditionalData($identityAdditionalData);

$source->setRegion(null);
$source->setLanguageId(null);
$sourceAdditionalData = [
"@odata.type" => '#microsoft.graph.participantInfo',
];
$source->setAdditionalData($sourceAdditionalData);

$targetsArray = [];

$targetstargets1 = new InvitationParticipantInfo();


$identity = new IdentitySet();
$targetstargets1->setIdentity($identity);



$user = new Identity();
$identity->setUser($user);


$user->setDisplayName('John');
$user->setId('112f7296-5fa4-42ca-bae8-6a692b15d4b8');
$userAdditionalData = [
"@odata.type" => '#microsoft.graph.identity',
];
$user->setAdditionalData($userAdditionalData);

$identityAdditionalData = [
"@odata.type" => '#microsoft.graph.identitySet',
];
$identity->setAdditionalData($identityAdditionalData);

$targetstargets1AdditionalData = [
"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
];
$targetstargets1->setAdditionalData($targetstargets1AdditionalData);

$targetsArray []= $targetstargets1;
$requestRequestBody->setTargets($targetsArray);
$requestedModalitiesArray = [];
'audio',$requestedModalitiesArray []= $requestedModalitiesrequestedModalities1;
$requestRequestBody->setRequestedModalities($requestedModalitiesArray);

$mediaConfig = new MediaConfig();
$requestRequestBody->setMediaConfig($mediaConfig);


$mediaConfigAdditionalData = [
"@odata.type" => '#microsoft.graph.appHostedMediaConfig',
"blob" => '<Media Session Configuration>',
];
$mediaConfig->setAdditionalData($mediaConfigAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.call',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->communications()->calls()->post($requestRequestBody);


```