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

$channelschannels1 = new Channel();

$channelschannels1->setDisplayName('Class Announcements 📢');
$channelschannels1->setIsFavoriteByDefault(True);

$channelsArray []= $channelschannels1;

$channelschannels2 = new Channel();

$channelschannels2->setDisplayName('Homework 🏋️');
$channelschannels2->setIsFavoriteByDefault(True);

$channelsArray []= $channelschannels2;
$requestRequestBody->setChannels($channelsArray);

$memberSettings = new TeamMemberSettings();
$requestRequestBody->setMemberSettings($memberSettings);


$memberSettings->setAllowCreateUpdateChannels(False);
$memberSettings->setAllowDeleteChannels(False);
$memberSettings->setAllowAddRemoveApps(False);
$memberSettings->setAllowCreateUpdateRemoveTabs(False);
$memberSettings->setAllowCreateUpdateRemoveConnectors(False);

$installedAppsArray = [];

$installedAppsinstalledApps1 = new TeamsAppInstallation();

$installedAppsinstalledApps1AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.vsts\')',
];
$installedAppsinstalledApps1->setAdditionalData($installedAppsinstalledApps1AdditionalData);

$installedAppsArray []= $installedAppsinstalledApps1;

$installedAppsinstalledApps2 = new TeamsAppInstallation();

$installedAppsinstalledApps2AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'1542629c-01b3-4a6d-8f76-1938b779e48d\')',
];
$installedAppsinstalledApps2->setAdditionalData($installedAppsinstalledApps2AdditionalData);

$installedAppsArray []= $installedAppsinstalledApps2;
$requestRequestBody->setInstalledApps($installedAppsArray);
$requestRequestBodyAdditionalData = [
"template@odata.bind" => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'educationClass\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```