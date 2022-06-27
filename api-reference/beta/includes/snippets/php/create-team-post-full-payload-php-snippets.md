---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Team();


$requestRequestBody->setVisibility(new TeamVisibilityType('Private'));
$requestRequestBody->setDisplayName('Sample Engineering Team');
$requestRequestBody->setDescription('This is a sample engineering team, used to showcase the range of properties supported by this API');
$channelsArray = [];

$channelschannels1 = new Channel();

$channelschannels1->setDisplayName('Announcements 📢');
$channelschannels1->setIsFavoriteByDefault(True);
$channelschannels1->setDescription('This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.');

$channelsArray []= $channelschannels1;

$channelschannels2 = new Channel();

$channelschannels2->setDisplayName('Training 🏋️');
$channelschannels2->setIsFavoriteByDefault(True);
$channelschannels2->setDescription('This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.');
$tabsArray = [];

$tabstabs1 = new TeamsTab();

$tabstabs1->setDisplayName('A Pinned Website');

$configuration = new TeamsTabConfiguration();
$tabstabs1->setConfiguration($configuration);


$configuration->setContentUrl('https://docs.microsoft.com/microsoftteams/microsoft-teams');

$tabstabs1AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.web\')',
];
$tabstabs1->setAdditionalData($tabstabs1AdditionalData);

$tabsArray []= $tabstabs1;

$tabstabs2 = new TeamsTab();

$tabstabs2->setDisplayName('A Pinned YouTube Video');

$configuration = new TeamsTabConfiguration();
$tabstabs2->setConfiguration($configuration);


$configuration->setContentUrl('https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ');
$configuration->setWebsiteUrl('https://www.youtube.com/watch?v=X8krAMdGvCQ');

$tabstabs2AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.youtube\')',
];
$tabstabs2->setAdditionalData($tabstabs2AdditionalData);

$tabsArray []= $tabstabs2;
$channelschannels2->setTabs($tabsArray);

$channelsArray []= $channelschannels2;

$channelschannels3 = new Channel();

$channelschannels3->setDisplayName('Planning 📅 ');
$channelschannels3->setDescription('This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.');
$channelschannels3->setIsFavoriteByDefault(False);

$channelsArray []= $channelschannels3;

$channelschannels4 = new Channel();

$channelschannels4->setDisplayName('Issues and Feedback 🐞');
$channelschannels4->setDescription('This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.');

$channelsArray []= $channelschannels4;
$requestRequestBody->setChannels($channelsArray);

$memberSettings = new TeamMemberSettings();
$requestRequestBody->setMemberSettings($memberSettings);


$memberSettings->setAllowCreateUpdateChannels(True);
$memberSettings->setAllowDeleteChannels(True);
$memberSettings->setAllowAddRemoveApps(True);
$memberSettings->setAllowCreateUpdateRemoveTabs(True);
$memberSettings->setAllowCreateUpdateRemoveConnectors(True);


$guestSettings = new TeamGuestSettings();
$requestRequestBody->setGuestSettings($guestSettings);


$guestSettings->setAllowCreateUpdateChannels(False);
$guestSettings->setAllowDeleteChannels(False);


$funSettings = new TeamFunSettings();
$requestRequestBody->setFunSettings($funSettings);


$funSettings->setAllowGiphy(True);
$funSettings->setGiphyContentRating(new GiphyRatingType('Moderate'));
$funSettings->setAllowStickersAndMemes(True);
$funSettings->setAllowCustomMemes(True);


$messagingSettings = new TeamMessagingSettings();
$requestRequestBody->setMessagingSettings($messagingSettings);


$messagingSettings->setAllowUserEditMessages(True);
$messagingSettings->setAllowUserDeleteMessages(True);
$messagingSettings->setAllowOwnerDeleteMessages(True);
$messagingSettings->setAllowTeamMentions(True);
$messagingSettings->setAllowChannelMentions(True);


$discoverySettings = new TeamDiscoverySettings();
$requestRequestBody->setDiscoverySettings($discoverySettings);


$discoverySettings->setShowInTeamsSearchAndSuggestions(True);

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
"template@odata.bind" => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```