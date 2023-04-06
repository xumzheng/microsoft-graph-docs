---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
channelsChannel1 = Channel()
channelsChannel1.setDisplayName('Class Announcements 📢')

channelsChannel1.setIsFavoriteByDefault(true)


channelsArray []= channelsChannel1;
channelsChannel2 = Channel()
channelsChannel2.setDisplayName('Homework 🏋️')

channelsChannel2.setIsFavoriteByDefault(true)


channelsArray []= channelsChannel2;
request_body.setChannels(channelsArray)


memberSettings = TeamMemberSettings()
memberSettings.setAllowCreateUpdateChannels(false)

memberSettings.setAllowDeleteChannels(false)

memberSettings.setAllowAddRemoveApps(false)

memberSettings.setAllowCreateUpdateRemoveTabs(false)

memberSettings.setAllowCreateUpdateRemoveConnectors(false)


request_body.setMemberSettings($memberSettings)
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
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
'group@odata.bind' => 'https://graph.microsoft.com/v1.0/groups(\'dbd8de4f-5d47-48da-87f1-594bed003375\')', 
];
request_body.setAdditionalData(additionalData)



request_config = TeamsRequestBuilderPostRequestConfiguration(
request_config = TeamsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams.post(request_body, headers=)


```