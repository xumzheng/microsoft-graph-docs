---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TeamsAppInstallation();
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.chatsById('chat-id').installedApps().post(requestBody);


```