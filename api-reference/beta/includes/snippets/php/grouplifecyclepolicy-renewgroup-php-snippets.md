---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GroupIdRequestBody();


$requestRequestBody->setGroupId('ffffffff-ffff-ffff-ffff-ffffffffffff');
$result =  $graphClient->groupLifecyclePolicies()->renewGroup()->post($requestRequestBody);


```