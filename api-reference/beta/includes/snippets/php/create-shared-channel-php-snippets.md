---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();


$requestRequestBody->setDisplayName('My First Shared Channel');
$requestRequestBody->setDescription('This is my first shared channel');
$requestRequestBody->setMembershipType(new ChannelMembershipType('shared'));
$membersArray = [];

$membersmembers1 = new ConversationMember();

$membersmembers1->setRoles(['owner',]);
$membersmembers1AdditionalData = [
"@odata.type" => '#microsoft.graph.aadUserConversationMember',
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'7640023f-fe43-gv3f-9gg4-84a9efe4acd6\')',
];
$membersmembers1->setAdditionalData($membersmembers1AdditionalData);

$membersArray []= $membersmembers1;
$requestRequestBody->setMembers($membersArray);
$result =  $graphClient->teamsById('team-id')->channels()->post($requestRequestBody);


```