---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.Visibility(TeamVisibilityType('private'))

request_body.displayName = 'Sample Engineering Team'

request_body.description = 'This is a sample engineering team, used to showcase the range of properties supported by this API'

channelsChannel1 = Channel()
channelsChannel1.displayName = 'Announcements 📢'

channelsChannel1.isFavoriteByDefault = true

channelsChannel1.description = 'This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.'


channelsArray []= channelsChannel1;
channelsChannel2 = Channel()
channelsChannel2.displayName = 'Training 🏋️'

channelsChannel2.isFavoriteByDefault = true

channelsChannel2.description = 'This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.'

tabsTeamsTab1 = TeamsTab()
tabsTeamsTab1.displayName = 'A Pinned Website'

tabsTeamsTab1Configuration = TeamsTabConfiguration()
tabsTeamsTab1Configuration.contentUrl = 'https://learn.microsoft.com/microsoftteams/microsoft-teams'


tabsTeamsTab1.configuration = tabsTeamsTab1Configuration
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.web\')', 
];
tabsTeamsTab1.additionaldata(additionalData)



tabsArray []= tabsTeamsTab1;
tabsTeamsTab2 = TeamsTab()
tabsTeamsTab2.displayName = 'A Pinned YouTube Video'

tabsTeamsTab2Configuration = TeamsTabConfiguration()
tabsTeamsTab2Configuration.contentUrl = 'https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ'

tabsTeamsTab2Configuration.websiteUrl = 'https://www.youtube.com/watch?v=X8krAMdGvCQ'


tabsTeamsTab2.configuration = tabsTeamsTab2Configuration
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.youtube\')', 
];
tabsTeamsTab2.additionaldata(additionalData)



tabsArray []= tabsTeamsTab2;
channelsChannel2.tabs(tabsArray)



channelsArray []= channelsChannel2;
channelsChannel3 = Channel()
channelsChannel3.displayName = 'Planning 📅 '

channelsChannel3.description = 'This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.'

channelsChannel3.isFavoriteByDefault = false


channelsArray []= channelsChannel3;
channelsChannel4 = Channel()
channelsChannel4.displayName = 'Issues and Feedback 🐞'

channelsChannel4.description = 'This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.'


channelsArray []= channelsChannel4;
request_body.channels(channelsArray)


memberSettings = TeamMemberSettings()
memberSettings.allowCreateUpdateChannels = true

memberSettings.allowDeleteChannels = true

memberSettings.allowAddRemoveApps = true

memberSettings.allowCreateUpdateRemoveTabs = true

memberSettings.allowCreateUpdateRemoveConnectors = true


request_body.memberSettings = memberSettings
guestSettings = TeamGuestSettings()
guestSettings.allowCreateUpdateChannels = false

guestSettings.allowDeleteChannels = false


request_body.guestSettings = guestSettings
funSettings = TeamFunSettings()
funSettings.allowGiphy = true

funSettings.GiphyContentRating(GiphyRatingType('moderate'))

funSettings.allowStickersAndMemes = true

funSettings.allowCustomMemes = true


request_body.funSettings = funSettings
messagingSettings = TeamMessagingSettings()
messagingSettings.allowUserEditMessages = true

messagingSettings.allowUserDeleteMessages = true

messagingSettings.allowOwnerDeleteMessages = true

messagingSettings.allowTeamMentions = true

messagingSettings.allowChannelMentions = true


request_body.messagingSettings = messagingSettings
installedAppsTeamsAppInstallation1 = TeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.vsts\')', 
];
installedAppsTeamsAppInstallation1.additionaldata(additionalData)



installedAppsArray []= installedAppsTeamsAppInstallation1;
installedAppsTeamsAppInstallation2 = TeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'1542629c-01b3-4a6d-8f76-1938b779e48d\')', 
];
installedAppsTeamsAppInstallation2.additionaldata(additionalData)



installedAppsArray []= installedAppsTeamsAppInstallation2;
request_body.installedapps(installedAppsArray)


additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
'discoverySettings' => request_body = DiscoverySettings()
request_body.showInTeamsSearchAndSuggestions = true


request_body.discoverySettings = discoverySettings

];
request_body.additionaldata(additionalData)





result = await client.teams.post(request_body = request_body)


```