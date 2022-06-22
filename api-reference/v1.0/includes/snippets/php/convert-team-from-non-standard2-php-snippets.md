---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Team();


$requestRequestBody->setDisplayName('My Class Team');
$requestRequestBody->setDescription('My Class Team’s Description');
$channelsArray = [];

$channels1 = new Channel();

$channels1->setDisplayName('Class Announcements 📢');
$channels1->setIsFavoriteByDefault(True);

$channelsArray []= $channels1;

$channels2 = new Channel();

$channels2->setDisplayName('Homework 🏋️');
$channels2->setIsFavoriteByDefault(True);

$channelsArray []= $channels2;
$requestRequestBody->setChannels($channelsArray);

$memberSettings = new TeamMemberSettings();
$requestRequestBody->setMemberSettings($memberSettings);


$memberSettings->setAllowCreateUpdateChannels(False);
$memberSettings->setAllowDeleteChannels(False);
$memberSettings->setAllowAddRemoveApps(False);
$memberSettings->setAllowCreateUpdateRemoveTabs(False);
$memberSettings->setAllowCreateUpdateRemoveConnectors(False);

$installedAppsArray = [];

$installedApps1 = new TeamsAppInstallation();

$installedApps1AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.vsts\')',
];
$installedApps1->setAdditionalData($installedApps1AdditionalData);

$installedAppsArray []= $installedApps1;

$installedApps2 = new TeamsAppInstallation();

$installedApps2AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'1542629c-01b3-4a6d-8f76-1938b779e48d\')',
];
$installedApps2->setAdditionalData($installedApps2AdditionalData);

$installedAppsArray []= $installedApps2;
$requestRequestBody->setInstalledApps($installedAppsArray);
$requestRequestBodyAdditionalData = [
"template@odata.bind" => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'educationClass\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```