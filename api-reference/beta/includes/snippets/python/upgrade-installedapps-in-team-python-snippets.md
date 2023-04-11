---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpgradePostRequestBody()
consentedPermissionSet = TeamsAppPermissionSet()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.permissionValue = 'Channel.Create.Group'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.PermissionType(TeamsAppResourceSpecificPermissionType('application'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission1;
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.permissionValue = 'ChannelMeeting.ReadBasic.Group'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.PermissionType(TeamsAppResourceSpecificPermissionType('delegated'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission2;
consentedPermissionSet.resourcespecificpermissions(resourceSpecificPermissionsArray)



request_body.consentedPermissionSet = consentedPermissionSet


request_configuration = UpgradeRequestBuilderPostRequestConfiguration(
)


await client.teams_by_id('team-id').installedApps_by_id('teamsAppInstallation-id').upgrade.post(request_body = request_body)


```