---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OAuth2PermissionGrant();
$requestBody->setScope('User.Read.All');



$requestResult = $graphServiceClient->oauth2PermissionGrantsById('oAuth2PermissionGrant-id')->patch($requestBody);


```