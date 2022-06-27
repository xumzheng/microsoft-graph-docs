---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Team();


$requestRequestBody->setDisplayName('My Sample Team');
$requestRequestBody->setDescription('My Sample Team’s Description');
$membersArray = [];

$membersmembers1 = new ConversationMember();

$membersmembers1->setRoles(['owner',]);
$membersmembers1AdditionalData = [
"@odata.type" => '#microsoft.graph.aadUserConversationMember',
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'0040b377-61d8-43db-94f5-81374122dc7e\')',
];
$membersmembers1->setAdditionalData($membersmembers1AdditionalData);

$membersArray []= $membersmembers1;
$requestRequestBody->setMembers($membersArray);
$requestRequestBodyAdditionalData = [
"template@odata.bind" => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```