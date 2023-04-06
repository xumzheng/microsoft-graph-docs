---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.setVisibility(TeamVisibilityType('private'))

request_body.setDisplayName('Sample Engineering Team')

request_body.setDescription('This is a sample engineering team, used to showcase the range of properties supported by this API')

channelsChannel1 = Channel()
channelsChannel1.setDisplayName('Announcements 📢')

channelsChannel1.setIsFavoriteByDefault(true)

channelsChannel1.setDescription('This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.')


channelsArray []= channelsChannel1;
channelsChannel2 = Channel()
channelsChannel2.setDisplayName('Training 🏋️')

channelsChannel2.setIsFavoriteByDefault(true)

channelsChannel2.setDescription('This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.')

tabsTeamsTab1 = TeamsTab()
tabsTeamsTab1.setDisplayName('A Pinned Website')

tabsTeamsTab1Configuration = TeamsTabConfiguration()
tabsTeamsTab1Configuration.setContentUrl('https://learn.microsoft.com/microsoftteams/microsoft-teams')


tabsTeamsTab1.setConfiguration($tabsTeamsTab1Configuration)
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.web\')', 
];
tabsTeamsTab1.setAdditionalData(additionalData)



tabsArray []= tabsTeamsTab1;
tabsTeamsTab2 = TeamsTab()
tabsTeamsTab2.setDisplayName('A Pinned YouTube Video')

tabsTeamsTab2Configuration = TeamsTabConfiguration()
tabsTeamsTab2Configuration.setContentUrl('https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ')

tabsTeamsTab2Configuration.setWebsiteUrl('https://www.youtube.com/watch?v=X8krAMdGvCQ')


tabsTeamsTab2.setConfiguration($tabsTeamsTab2Configuration)
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.youtube\')', 
];
tabsTeamsTab2.setAdditionalData(additionalData)



tabsArray []= tabsTeamsTab2;
channelsChannel2.setTabs(tabsArray)



channelsArray []= channelsChannel2;
channelsChannel3 = Channel()
channelsChannel3.setDisplayName('Planning 📅 ')

channelsChannel3.setDescription('This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.')

channelsChannel3.setIsFavoriteByDefault(false)


channelsArray []= channelsChannel3;
channelsChannel4 = Channel()
channelsChannel4.setDisplayName('Issues and Feedback 🐞')

channelsChannel4.setDescription('This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.')


channelsArray []= channelsChannel4;
request_body.setChannels(channelsArray)


memberSettings = TeamMemberSettings()
memberSettings.setAllowCreateUpdateChannels(true)

memberSettings.setAllowDeleteChannels(true)

memberSettings.setAllowAddRemoveApps(true)

memberSettings.setAllowCreateUpdateRemoveTabs(true)

memberSettings.setAllowCreateUpdateRemoveConnectors(true)


request_body.setMemberSettings($memberSettings)
guestSettings = TeamGuestSettings()
guestSettings.setAllowCreateUpdateChannels(false)

guestSettings.setAllowDeleteChannels(false)


request_body.setGuestSettings($guestSettings)
funSettings = TeamFunSettings()
funSettings.setAllowGiphy(true)

funSettings.setGiphyContentRating(GiphyRatingType('moderate'))

funSettings.setAllowStickersAndMemes(true)

funSettings.setAllowCustomMemes(true)


request_body.setFunSettings($funSettings)
messagingSettings = TeamMessagingSettings()
messagingSettings.setAllowUserEditMessages(true)

messagingSettings.setAllowUserDeleteMessages(true)

messagingSettings.setAllowOwnerDeleteMessages(true)

messagingSettings.setAllowTeamMentions(true)

messagingSettings.setAllowChannelMentions(true)


request_body.setMessagingSettings($messagingSettings)
discoverySettings = TeamDiscoverySettings()
discoverySettings.setShowInTeamsSearchAndSuggestions(true)


request_body.setDiscoverySettings($discoverySettings)
installedAppsTeamsAppInstallation1 = TeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.vsts\')', 
];
installedAppsTeamsAppInstallation1.setAdditionalData(additionalData)



installedAppsArray []= installedAppsTeamsAppInstallation1;
installedAppsTeamsAppInstallation2 = TeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'1542629c-01b3-4a6d-8f76-1938b779e48d\')', 
];
installedAppsTeamsAppInstallation2.setAdditionalData(additionalData)



installedAppsArray []= installedAppsTeamsAppInstallation2;
request_body.setInstalledApps(installedAppsArray)


additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')', 
];
request_body.setAdditionalData(additionalData)




result = await client.teams.post(request_body, headers=)


```