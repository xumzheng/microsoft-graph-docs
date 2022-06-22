---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RejectPostRequestBody();


$requestRequestBody->setReason(new RejectReason('busy'));
$result =  $graphClient->communications()->callsById('call-id')->reject()->post($requestRequestBody);


```