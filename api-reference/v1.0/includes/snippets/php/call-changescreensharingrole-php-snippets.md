---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RoleRequestBody();


$requestRequestBody->setRole(new ScreenSharingRole('viewer'));
$result =  $graphClient->communications()->callsById('call-id')->changeScreenSharingRole()->post($requestRequestBody);


```