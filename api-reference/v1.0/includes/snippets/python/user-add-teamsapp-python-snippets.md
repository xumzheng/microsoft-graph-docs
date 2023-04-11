---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserScopeTeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a', 
];
request_body.additionaldata(additionalData)




request_configuration = InstalledAppsRequestBuilderPostRequestConfiguration(
)


result = await client.users_by_id('user-id').teamwork.installedApps.post(request_body = request_body)


```