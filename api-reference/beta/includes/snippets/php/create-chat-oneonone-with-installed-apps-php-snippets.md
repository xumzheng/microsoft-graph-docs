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
		"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')',
	];
$members1->setAdditionalData($members1AdditionalData);

$membersArray []= $members1;

$members2 = new ConversationMember();

$members2->setRoles( [
'owner',],
$members2AdditionalData = [
	"@odata.type" => '#microsoft.graph.aadUserConversationMember',
	"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'82af01c5-f7cc-4a2e-a728-3a5df21afd9d\')',
];
$members2->setAdditionalData($members2AdditionalData);

$membersArray []= $members2;
$requestRequestBody->setMembers($membersArray);
$installedAppsArray = [];

$installedApps1 = new TeamsAppInstallation();

$installedApps1AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4',
];
$installedApps1->setAdditionalData($installedApps1AdditionalData);

$installedAppsArray []= $installedApps1;
$requestRequestBody->setInstalledApps($installedAppsArray);
$result =  $graphClient->chats()->post($requestRequestBody);


```