---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Chat();


$requestRequestBody->setChatType(new ChatType('oneOnOne'));
$membersArray = [];

$members1 = new ConversationMember();

$members1->setRoles( [
'owner',	],
$members1AdditionalData = [
		"@odata.type" => '#microsoft.graph.aadUserConversationMember',
		"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')',
	];
$members1->setAdditionalData($members1AdditionalData);

$membersArray []= $members1;

$members2 = new ConversationMember();

$members2->setRoles( [
'owner',],
$members2AdditionalData = [
	"@odata.type" => '#microsoft.graph.aadUserConversationMember',
	"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'alex@contoso.com\')',
];
$members2->setAdditionalData($members2AdditionalData);

$membersArray []= $members2;
$requestRequestBody->setMembers($membersArray);
$result =  $graphClient->chats()->post($requestRequestBody);


```