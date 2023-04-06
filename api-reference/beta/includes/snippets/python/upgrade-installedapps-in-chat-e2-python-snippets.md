---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpgradePostRequestBody()
consentedPermissionSet = TeamsAppPermissionSet()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.setPermissionValue('OnlineMeeting.ReadBasic.Chat')

resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.setPermissionType(TeamsAppResourceSpecificPermissionType('delegated'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission1;
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.setPermissionValue('ChatMember.Read.Chat')

resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.setPermissionType(TeamsAppResourceSpecificPermissionType('application'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission2;
consentedPermissionSet.setResourceSpecificPermissions(resourceSpecificPermissionsArray)



request_body.setConsentedPermissionSet($consentedPermissionSet)


await client.chats_by_id('chat-id').installedApps_by_id('teamsAppInstallation-id').upgrade.post(request_body, headers=)


```