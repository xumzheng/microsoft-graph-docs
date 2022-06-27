---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SessionIdRequestBody();


$requestRequestBody->setSessionId('22553876-f5ab-4529-bffb-cfe50aa89f87');
$result =  $graphClient->usersById('user-id')->presence()->clearPresence()->post($requestRequestBody);


```