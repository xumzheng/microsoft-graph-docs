---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Chat();


$requestRequestBody->setChatType(new ChatType('group'));
$requestRequestBody->setTopic('Group chat title');
$membersArray = [];

$members1 = new ConversationMember();

$members1->setRoles( [
'owner',	],
$members1AdditionalData = [
		"@odata.type" => '#microsoft.graph.aadUserConversationMember',
		"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca\')',
	];
$members1->setAdditionalData($members1AdditionalData);

$membersArray []= $members1;

$members2 = new ConversationMember();

$members2->setRoles( [
'owner',],
$members2AdditionalData = [
	"@odata.type" => '#microsoft.graph.aadUserConversationMember',
	"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'82fe7758-5bb3-4f0d-a43f-e555fd399c6f\')',
];
$members2->setAdditionalData($members2AdditionalData);

$membersArray []= $members2;

$members3 = new ConversationMember();

$members3->setRoles( [
'guest',],
$members3AdditionalData = [
"@odata.type" => '#microsoft.graph.aadUserConversationMember',
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'8ba98gf6-7fc2-4eb2-c7f2-aef9f21fd98g\')',
];
$members3->setAdditionalData($members3AdditionalData);

$membersArray []= $members3;
$requestRequestBody->setMembers($membersArray);
$result =  $graphClient->chats()->post($requestRequestBody);


```