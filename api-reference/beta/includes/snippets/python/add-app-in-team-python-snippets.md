---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TeamsAppInstallation();
$additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a', 
];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.teamsById('team-id').installedApps().post($requestBody);


```