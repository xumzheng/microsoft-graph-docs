---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UserScopeTeamsAppInstallation();
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.usersById('user-id').teamwork().installedApps().post(requestBody);


```