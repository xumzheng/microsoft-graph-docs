---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DestinationIdRequestBody();


$requestRequestBody->setDestinationId('destinationId-value');
$result =  $graphClient->me()->mailFoldersById('mailFolder-id')->move()->post($requestRequestBody);


```