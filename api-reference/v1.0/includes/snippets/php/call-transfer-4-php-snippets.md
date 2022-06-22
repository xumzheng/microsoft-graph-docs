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


$identityAdditionalData = [
	"@odata.type" => '#microsoft.graph.identitySet',
];
$identity->setAdditionalData($identityAdditionalData);

$transferTarget->setReplacesCallId('e5d39592-99bd-4db8-bca8-30fb894ec51d');
$transferTargetAdditionalData = [
"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
"endpointType" => 'default',
"languageId" => 'en-us',
"region" => 'amer',
];
$transferTarget->setAdditionalData($transferTargetAdditionalData);

$requestRequestBodyAdditionalData = [
"clientContext" => '9e90d1c1-f61e-43e7-9f75-d420159aae08',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->communications()->callsById('call-id')->transfer()->post($requestRequestBody);


```