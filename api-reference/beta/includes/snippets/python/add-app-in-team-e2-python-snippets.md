---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsAppInstallation()
consentedPermissionSet = TeamsAppPermissionSet()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.permissionValue = 'OnlineMeeting.ReadBasic.Chat'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission1.PermissionType(TeamsAppResourceSpecificPermissionType('delegated'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission1;
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2 = TeamsAppResourceSpecificPermission()
resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.permissionValue = 'ChatMessage.Read.Chat'

resourceSpecificPermissionsTeamsAppResourceSpecificPermission2.PermissionType(TeamsAppResourceSpecificPermissionType('application'))


resourceSpecificPermissionsArray []= resourceSpecificPermissionsTeamsAppResourceSpecificPermission2;
consentedPermissionSet.resourcespecificpermissions(resourceSpecificPermissionsArray)



request_body.consentedPermissionSet = consentedPermissionSet
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/7023576d-9e40-47ca-9cf2-daae6838e785', 
];
request_body.additionaldata(additionalData)





result = await client.teams_by_id('team-id').installedApps.post(request_body = request_body)


```