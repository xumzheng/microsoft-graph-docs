---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ClientContextRequestBody();


$requestRequestBody->setClientContext('d45324c1-fcb5-430a-902c-f20af696537c');
$result =  $graphClient->communications()->callsById('call-id')->participantsById('participant-id')->mute()->post($requestRequestBody);


```