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

$channels1 = new Channel();

$channels1->setDisplayName('Announcements 📢');
$channels1->setIsFavoriteByDefault(True);
$channels1->setDescription('This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.');

$channelsArray []= $channels1;

$channels2 = new Channel();

$channels2->setDisplayName('Training 🏋️');
$channels2->setIsFavoriteByDefault(True);
$channels2->setDescription('This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.');
$tabsArray = [];

$tabs1 = new TeamsTab();

$tabs1->setDisplayName('A Pinned Website');

$configuration = new TeamsTabConfiguration();
$tabs1->setConfiguration($configuration);


$configuration->setContentUrl('https://docs.microsoft.com/microsoftteams/microsoft-teams');

$tabs1AdditionalData = [
	"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.web\')',
];
$tabs1->setAdditionalData($tabs1AdditionalData);

$tabsArray []= $tabs1;

$tabs2 = new TeamsTab();

$tabs2->setDisplayName('A Pinned YouTube Video');

$configuration = new TeamsTabConfiguration();
$tabs2->setConfiguration($configuration);


$configuration->setContentUrl('https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ');
$configuration->setWebsiteUrl('https://www.youtube.com/watch?v=X8krAMdGvCQ');

$tabs2AdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.youtube\')',
];
$tabs2->setAdditionalData($tabs2AdditionalData);

$tabsArray []= $tabs2;
$channels2->setTabs($tabsArray);

$channelsArray []= $channels2;

$channels3 = new Channel();

$channels3->setDisplayName('Planning 📅 ');
$channels3->setDescription('This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.');
$channels3->setIsFavoriteByDefault(False);

$channelsArray []= $channels3;

$channels4 = new Channel();

$channels4->setDisplayName('Issues and Feedback 🐞');
$channels4->setDescription('This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.');

$channelsArray []= $channels4;
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
"template@odata.bind" => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```