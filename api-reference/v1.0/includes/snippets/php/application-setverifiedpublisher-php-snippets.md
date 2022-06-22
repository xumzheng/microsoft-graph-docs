---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new VerifiedPublisherIdRequestBody();


$requestRequestBody->setVerifiedPublisherId('1234567');
$result =  $graphClient->applicationsById('application-id')->setVerifiedPublisher()->post($requestRequestBody);


```