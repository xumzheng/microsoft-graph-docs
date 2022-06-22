---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SetPresencePostRequestBody();


$requestRequestBody->setSessionId('22553876-f5ab-4529-bffb-cfe50aa89f87');
$requestRequestBody->setAvailability('Available');
$requestRequestBody->setActivity('Available');
$requestRequestBody->setExpirationDuration('PT1H');
$result =  $graphClient->usersById('user-id')->presence()->setPresence()->post($requestRequestBody);


```