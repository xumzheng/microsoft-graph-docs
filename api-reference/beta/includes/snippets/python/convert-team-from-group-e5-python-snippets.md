---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
channels_channel1 = Channel()
channelsChannel1.displayName = 'Class Announcements 📢'

channelsChannel1.is_favorite_by_default = True


channelsArray []= channelsChannel1;
channels_channel2 = Channel()
channelsChannel2.displayName = 'Homework 🏋️'

channelsChannel2.is_favorite_by_default = True


channelsArray []= channelsChannel2;
request_body.channels(channelsArray)


member_settings = TeamMemberSettings()
memberSettings.allow_create_update_channels = False

memberSettings.allow_delete_channels = False

memberSettings.allow_add_remove_apps = False

memberSettings.allow_create_update_remove_tabs = False

memberSettings.allow_create_update_remove_connectors = False


request_body.member_settings = memberSettings
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
'template@odata.bind' => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')', 
'group@odata.bind' => 'https://graph.microsoft.com/beta/groups(\'dbd8de4f-5d47-48da-87f1-594bed003375\')', 
];
request_body.additionaldata(additionalData)





result = await client.teams.post(request_body = request_body)


```