---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InvitePostRequestBody();


$participantsArray = [];

$participantsparticipants1 = new InvitationParticipantInfo();

$participantsparticipants1AdditionalData = [
	"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
];
$participantsparticipants1->setAdditionalData($participantsparticipants1AdditionalData);

$participantsArray []= $participantsparticipants1;
$requestRequestBody->setParticipants($participantsArray);
$requestRequestBody->setClientContext('f2fa86af-3c51-4bc2-8fc0-475452d9764f');
$result =  $graphClient->communications()->callsById('call-id')->participants()->invite()->post($requestRequestBody);


```