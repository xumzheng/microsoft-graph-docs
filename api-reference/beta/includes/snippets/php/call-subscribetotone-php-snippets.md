---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ClientContextRequestBody();


$requestRequestBody->setClientContext('fd1c7836-4d84-4e24-b6aa-23188688cc54');
$result =  $graphClient->communications()->callsById('call-id')->subscribeToTone()->post($requestRequestBody);


```