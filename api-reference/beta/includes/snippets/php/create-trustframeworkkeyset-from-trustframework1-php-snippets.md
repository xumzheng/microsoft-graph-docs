---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TrustFrameworkKeySet();


$requestRequestBody->setId('keyset1');
$result =  $graphClient->trustFramework()->keySets()->post($requestRequestBody);


```