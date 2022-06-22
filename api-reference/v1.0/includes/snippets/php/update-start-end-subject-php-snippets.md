---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OnlineMeeting();


$requestRequestBody->setStartDateTime(new DateTime("2020-09-09T14:33:30.8546353-07:00"));
$requestRequestBody->setEndDateTime(new DateTime("2020-09-09T15:03:30.8566356-07:00"));
$requestRequestBody->setSubject('Patch Meeting Subject');
$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->patch($requestRequestBody);


```