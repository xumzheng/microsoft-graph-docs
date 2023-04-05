---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpgradePostRequestBody()
consentedPermissionSet = TeamsAppPermissionSet()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.setPermissionValue('Channel.Create.Group')

resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.setPermissionType(TeamsAppResourceSpecificPermissionType('application'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission1;
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.setPermissionValue('ChannelMeeting.ReadBasic.Group')

resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.setPermissionType(TeamsAppResourceSpecificPermissionType('delegated'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission2;
consentedPermissionSet.setResourceSpecificPermissions(resourceSpecificPermissionsArray)



request_body.setConsentedPermissionSet($consentedPermissionSet)


await client.teams_by_id('team-id').installedApps_by_id('teamsAppInstallation-id').upgrade.post(request_body)


```