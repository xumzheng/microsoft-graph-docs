---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ClockOutPostRequestBody();



$notes = new ItemBody();
$requestRequestBody->setNotes($notes);


$notes->setContentType(new BodyType('text'));
$notes->setContent('clock out smaple notes');

$requestRequestBodyAdditionalData = [
"atAprovedLocation" => True,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->schedule()->timeCardsById('timeCard-id')->clockOut()->post($requestRequestBody);


```