---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsAppInstallation()
consentedPermissionSet = TeamsAppPermissionSet()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.setPermissionValue('OnlineMeeting.ReadBasic.Chat')

resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.setPermissionType(TeamsAppResourceSpecificPermissionType('delegated'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission1;
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.setPermissionValue('ChatMessage.Read.Chat')

resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.setPermissionType(TeamsAppResourceSpecificPermissionType('application'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission2;
consentedPermissionSet.setResourceSpecificPermissions(resourceSpecificPermissionsArray)



request_body.setConsentedPermissionSet($consentedPermissionSet)
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/7023576d-9e40-47ca-9cf2-daae6838e785', 
];
request_body.setAdditionalData(additionalData)



request_config = InstalledAppsRequestBuilderPostRequestConfiguration(
request_config = InstalledAppsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').installedApps.post(request_body, headers=)


```