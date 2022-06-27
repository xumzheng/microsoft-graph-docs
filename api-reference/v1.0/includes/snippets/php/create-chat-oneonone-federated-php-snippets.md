---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Chat();


$requestRequestBody->setChatType(new ChatType('oneOnOne'));
$membersArray = [];

$membersmembers1 = new ConversationMember();

$membersmembers1->setRoles(['owner',]);
$membersmembers1AdditionalData = [
"@odata.type" => '#microsoft.graph.aadUserConversationMember',
"user@odata.bind" => 'https://graph.microsoft.com/v1.0/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')',
];
$membersmembers1->setAdditionalData($membersmembers1AdditionalData);

$membersArray []= $membersmembers1;

$membersmembers2 = new ConversationMember();

$membersmembers2->setRoles(['owner',]);
$membersmembers2AdditionalData = [
"@odata.type" => '#microsoft.graph.aadUserConversationMember',
"user@odata.bind" => 'https://graph.microsoft.com/v1.0/users(\'82af01c5-f7cc-4a2e-a728-3a5df21afd9d\')',
"tenantId" => '4dc1fe35-8ac6-4f0d-904a-7ebcd364bea1',
];
$membersmembers2->setAdditionalData($membersmembers2AdditionalData);

$membersArray []= $membersmembers2;
$requestRequestBody->setMembers($membersArray);
$result =  $graphClient->chats()->post($requestRequestBody);


```