---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PermissionGrantPolicy();


$requestRequestBody->setDisplayName('Custom permission grant policy');
$result =  $graphClient->policies()->permissionGrantPoliciesById('permissionGrantPolicy-id')->patch($requestRequestBody);


```