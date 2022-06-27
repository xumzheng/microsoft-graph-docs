---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DestinationIdRequestBody();


$requestRequestBody->setDestinationId('deleteditems');
$result =  $graphClient->me()->messagesById('message-id')->move()->post($requestRequestBody);


```