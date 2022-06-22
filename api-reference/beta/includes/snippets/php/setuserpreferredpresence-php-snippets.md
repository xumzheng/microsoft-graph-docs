---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SetUserPreferredPresencePostRequestBody();


$requestRequestBody->setAvailability('DoNotDisturb');
$requestRequestBody->setActivity('DoNotDisturb');
$requestRequestBody->setExpirationDuration('PT8H');
$result =  $graphClient->usersById('user-id')->presence()->setUserPreferredPresence()->post($requestRequestBody);


```