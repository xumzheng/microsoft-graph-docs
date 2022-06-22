---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RegistrationPostRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.externalMeetingRegistration',
	"allowedRegistrant" => 'everyone',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->post($requestRequestBody);


```