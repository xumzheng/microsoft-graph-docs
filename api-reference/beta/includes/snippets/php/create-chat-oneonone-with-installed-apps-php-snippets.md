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
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')',
];
$membersmembers1->setAdditionalData($membersmembers1AdditionalData);

$membersArray []= $membersmembers1;

$membersmembers2 = new ConversationMember();

$membersmembers2->setRoles(['owner',]);
$membersmembers2AdditionalData = [
"@odata.type" => '#microsoft.graph.aadUserConversationMember',
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'82af01c5-f7cc-4a2e-a728-3a5df21afd9d\')',
];
$membersmembers2->setAdditionalData($membersmembers2AdditionalData);

$membersArray []= $membersmembers2;
$requestRequestBody->setMembers($membersArray);
$installedAppsArray = [];

$installedAppsinstalledApps1 = new TeamsAppInstallation();

$installedAppsinstalledApps1AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4',
];
$installedAppsinstalledApps1->setAdditionalData($installedAppsinstalledApps1AdditionalData);

$installedAppsArray []= $installedAppsinstalledApps1;
$requestRequestBody->setInstalledApps($installedAppsArray);
$result =  $graphClient->chats()->post($requestRequestBody);


```