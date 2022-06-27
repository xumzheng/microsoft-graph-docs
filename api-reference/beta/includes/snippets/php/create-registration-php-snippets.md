---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RegistrationPostRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.meetingRegistration',
	"subject" => 'Microsoft Ignite',
	"description" => 'Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.',
	"startDateTime" => '2021-11-02T08:00:00-08:00',
	"endDateTime" => '2021-11-04T04:00:00-08:00',
	"allowedRegistrant" => 'everyone',
	"speakers" => [],
"customQuestions" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->post($requestRequestBody);


```