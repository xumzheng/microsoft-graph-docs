---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OAuth2PermissionGrant();


$requestRequestBody->setScope('User.ReadBasic.All Group.ReadWrite.All');
$result =  $graphClient->oauth2PermissionGrantsById('oAuth2PermissionGrant-id')->patch($requestRequestBody);


```