---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PermissionGrantConditionSet();


$requestRequestBody->setPermissionType(new PermissionType('delegated'));
$requestRequestBody->setResourceApplication('00000003-0000-0000-c000-000000000000');
$result =  $graphClient->policies()->permissionGrantPoliciesById('permissionGrantPolicy-id')->excludes()->post($requestRequestBody);


```