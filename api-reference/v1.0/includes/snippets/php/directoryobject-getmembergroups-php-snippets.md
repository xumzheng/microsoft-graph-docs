---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SecurityEnabledOnlyRequestBody();


$requestRequestBody->setSecurityEnabledOnly(False);
$result =  $graphClient->directoryObjectsById('directoryObject-id')->getMemberGroups()->post($requestRequestBody);


```