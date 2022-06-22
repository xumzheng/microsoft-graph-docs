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
];
$identity->setAdditionalData($identityAdditionalData);

$transferTargetAdditionalData = [
"endpointType" => 'default',
"languageId" => 'languageId-value',
"region" => 'region-value',
];
$transferTarget->setAdditionalData($transferTargetAdditionalData);

$requestRequestBodyAdditionalData = [
"clientContext" => '9e90d1c1-f61e-43e7-9f75-d420159aae08',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->communications()->callsById('call-id')->transfer()->post($requestRequestBody);


```