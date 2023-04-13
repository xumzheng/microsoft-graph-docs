---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsAppInstallation()
consented_permission_set = TeamsAppPermissionSet()
resource_specific_permissions_teams_app_resource_specific_permission1 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.permissionValue = 'OnlineMeeting.ReadBasic.Chat'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.PermissionType(TeamsAppResourceSpecificPermissionType('delegated'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission1;
resource_specific_permissions_teams_app_resource_specific_permission2 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.permissionValue = 'OnlineMeetingIncomingAudio.Detect.Chat'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.PermissionType(TeamsAppResourceSpecificPermissionType('delegated'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission2;
resource_specific_permissions_teams_app_resource_specific_permission3 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission3.permissionValue = 'ChatMember.Read.Chat'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission3.PermissionType(TeamsAppResourceSpecificPermissionType('application'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission3;
resource_specific_permissions_teams_app_resource_specific_permission4 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission4.permissionValue = 'ChatMessage.Read.Chat'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission4.PermissionType(TeamsAppResourceSpecificPermissionType('application'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission4;
consentedPermissionSet.resourcespecificpermissions(resourceSpecificPermissionsArray)



request_body.consented_permission_set = consentedPermissionSet
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/2b524e28-95ce-4c9b-9773-4a5bd6ec1770', 
];
request_body.additionaldata(additionalData)





result = await client.chats_by_id('chat-id').installedApps.post(request_body = request_body)


```