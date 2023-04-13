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

channels_channel1 = Channel()
channelsChannel1.displayName = 'Announcements 📢'

channelsChannel1.is_favorite_by_default = True

channelsChannel1.description = 'This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.'


channelsArray []= channelsChannel1;
channels_channel2 = Channel()
channelsChannel2.displayName = 'Training 🏋️'

channelsChannel2.is_favorite_by_default = True

channelsChannel2.description = 'This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.'

tabs_teams_tab1 = TeamsTab()
tabsTeamsTab1.displayName = 'A Pinned Website'

tabs_teams_tab1_configuration = TeamsTabConfiguration()
tabsTeamsTab1Configuration.contentUrl = 'https://learn.microsoft.com/microsoftteams/microsoft-teams'


tabsTeamsTab1.configuration = tabsTeamsTab1Configuration
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.web\')', 
];
tabsTeamsTab1.additionaldata(additionalData)



tabsArray []= tabsTeamsTab1;
tabs_teams_tab2 = TeamsTab()
tabsTeamsTab2.displayName = 'A Pinned YouTube Video'

tabs_teams_tab2_configuration = TeamsTabConfiguration()
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
channels_channel3 = Channel()
channelsChannel3.displayName = 'Planning 📅 '

channelsChannel3.description = 'This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.'

channelsChannel3.is_favorite_by_default = False


channelsArray []= channelsChannel3;
channels_channel4 = Channel()
channelsChannel4.displayName = 'Issues and Feedback 🐞'

channelsChannel4.description = 'This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.'


channelsArray []= channelsChannel4;
request_body.channels(channelsArray)


member_settings = TeamMemberSettings()
memberSettings.allow_create_update_channels = True

memberSettings.allow_delete_channels = True

memberSettings.allow_add_remove_apps = True

memberSettings.allow_create_update_remove_tabs = True

memberSettings.allow_create_update_remove_connectors = True


request_body.member_settings = memberSettings
guest_settings = TeamGuestSettings()
guestSettings.allow_create_update_channels = False

guestSettings.allow_delete_channels = False


request_body.guest_settings = guestSettings
fun_settings = TeamFunSettings()
funSettings.allow_giphy = True

funSettings.GiphyContentRating(GiphyRatingType('moderate'))

funSettings.allow_stickers_and_memes = True

funSettings.allow_custom_memes = True


request_body.fun_settings = funSettings
messaging_settings = TeamMessagingSettings()
messagingSettings.allow_user_edit_messages = True

messagingSettings.allow_user_delete_messages = True

messagingSettings.allow_owner_delete_messages = True

messagingSettings.allow_team_mentions = True

messagingSettings.allow_channel_mentions = True


request_body.messaging_settings = messagingSettings
installed_apps_teams_app_installation1 = TeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.vsts\')', 
];
installedAppsTeamsAppInstallation1.additionaldata(additionalData)



installedAppsArray []= installedAppsTeamsAppInstallation1;
installed_apps_teams_app_installation2 = TeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'1542629c-01b3-4a6d-8f76-1938b779e48d\')', 
];
installedAppsTeamsAppInstallation2.additionaldata(additionalData)



installedAppsArray []= installedAppsTeamsAppInstallation2;
request_body.installedapps(installedAppsArray)


additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
'discoverySettings' => request_body = DiscoverySettings()
request_body.show_in_teams_search_and_suggestions = True


request_body.discovery_settings = discoverySettings

];
request_body.additionaldata(additionalData)





result = await client.teams.post(request_body = request_body)


```