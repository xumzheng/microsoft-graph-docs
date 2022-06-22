---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OnlineMeeting();


$requestRequestBody->setStartDateTime(new DateTime("2019-07-12T14:30:34.2444915-07:00"));
$requestRequestBody->setEndDateTime(new DateTime("2019-07-12T15:00:34.2464912-07:00"));
$requestRequestBody->setSubject('User Token Meeting');
$result =  $graphClient->me()->onlineMeetings()->post($requestRequestBody);


```