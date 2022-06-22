---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UploadSecretPostRequestBody();


$requestRequestBody->setUse('use-value');
$requestRequestBody->setK('application-secret-to-be-uploaded');
$requestRequestBody->setNbf(1508969811);
$requestRequestBody->setExp(1508973711);
$result =  $graphClient->trustFramework()->keySetsById('trustFrameworkKeySet-id')->uploadSecret()->post($requestRequestBody);


```