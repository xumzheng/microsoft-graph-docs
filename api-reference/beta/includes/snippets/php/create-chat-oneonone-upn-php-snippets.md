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
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')',
];
$membersmembers1->setAdditionalData($membersmembers1AdditionalData);

$membersArray []= $membersmembers1;

$membersmembers2 = new ConversationMember();

$membersmembers2->setRoles(['owner',]);
$membersmembers2AdditionalData = [
"@odata.type" => '#microsoft.graph.aadUserConversationMember',
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'alex@contoso.com\')',
];
$membersmembers2->setAdditionalData($membersmembers2AdditionalData);

$membersArray []= $membersmembers2;
$requestRequestBody->setMembers($membersArray);
$result =  $graphClient->chats()->post($requestRequestBody);


```