---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OAuth2PermissionGrant();
requestBody.setScope('User.Read.All');



result = awaitclient.oauth2PermissionGrantsById('oAuth2PermissionGrant-id').patch(requestBody);


```