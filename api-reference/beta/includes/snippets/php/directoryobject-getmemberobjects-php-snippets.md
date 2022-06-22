---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SecurityEnabledOnlyRequestBody();


$requestRequestBody->setSecurityEnabledOnly(True);
$result =  $graphClient->me()->getMemberObjects()->post($requestRequestBody);


```