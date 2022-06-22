---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();


$requestRequestBody->setMembershipType(new ChannelMembershipType('private'));
$requestRequestBody->setDisplayName('My First Private Channel');
$requestRequestBody->setDescription('This is my first private channels');
$membersArray = [];

$members1 = new ConversationMember();

$members1->setRoles( [
'owner',	],
$members1AdditionalData = [
		"@odata.type" => '#microsoft.graph.aadUserConversationMember',
		"user@odata.bind" => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')',
	];
$members1->setAdditionalData($members1AdditionalData);

$membersArray []= $members1;
$requestRequestBody->setMembers($membersArray);
$requestRequestBodyAdditionalData = [
"@odata.type" => '#Microsoft.Graph.channel',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->channels()->post($requestRequestBody);


```