---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InvitePostRequestBody();


$participantsArray = [];

$participants1 = new InvitationParticipantInfo();

$participants1AdditionalData = [
		"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
		"replacesCallId" => 'a7ebfb2d-871e-419c-87af-27290b22e8db',
	];
$participants1->setAdditionalData($participants1AdditionalData);

$participantsArray []= $participants1;
$requestRequestBody->setParticipants($participantsArray);
$requestRequestBody->setClientContext('f2fa86af-3c51-4bc2-8fc0-475452d9764f');
$result =  $graphClient->communications()->callsById('call-id')->participants()->invite()->post($requestRequestBody);


```