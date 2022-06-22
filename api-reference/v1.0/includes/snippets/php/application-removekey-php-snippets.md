---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RemoveKeyPostRequestBody();


$requestRequestBody->setKeyId('f0b0b335-1d71-4883-8f98-567911bfdca6');
$requestRequestBody->setProof('eyJ0eXAiOiJ...');
$result =  $graphClient->applicationsById('application-id')->removeKey()->post($requestRequestBody);


```