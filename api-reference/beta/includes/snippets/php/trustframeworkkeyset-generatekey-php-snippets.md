---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GenerateKeyPostRequestBody();


$requestRequestBody->setUse('sig');
$requestRequestBody->setKty('RSA');
$requestRequestBody->setNbf(1508969811);
$requestRequestBody->setExp(1508969811);
$result =  $graphClient->trustFramework()->keySetsById('trustFrameworkKeySet-id')->generateKey()->post($requestRequestBody);


```