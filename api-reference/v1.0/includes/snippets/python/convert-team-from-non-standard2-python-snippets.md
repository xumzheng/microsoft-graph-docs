---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.displayName = 'My Class Team'

request_body.description = 'My Class Team’s Description'

channelsChannel1 = Channel()
channelsChannel1.displayName = 'Class Announcements 📢'

channelsChannel1.isFavoriteByDefault = true


channelsArray []= channelsChannel1;
channelsChannel2 = Channel()
channelsChannel2.displayName = 'Homework 🏋️'

channelsChannel2.isFavoriteByDefault = true


channelsArray []= channelsChannel2;
request_body.channels(channelsArray)


memberSettings = TeamMemberSettings()
memberSettings.allowCreateUpdateChannels = false

memberSettings.allowDeleteChannels = false

memberSettings.allowAddRemoveApps = false

memberSettings.allowCreateUpdateRemoveTabs = false

memberSettings.allowCreateUpdateRemoveConnectors = false


request_body.memberSettings = memberSettings
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
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'educationClass\')', 
];
request_body.additionaldata(additionalData)





result = await client.teams.post(request_body = request_body)


```