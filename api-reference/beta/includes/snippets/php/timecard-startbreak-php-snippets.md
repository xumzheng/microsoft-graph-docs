---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new StartBreakPostRequestBody();



$notes = new ItemBody();
$requestRequestBody->setNotes($notes);


$notes->setContentType(new BodyType('text'));
$notes->setContent('start break smaple notes');

$requestRequestBodyAdditionalData = [
"atAprovedLocation" => True,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->schedule()->timeCardsById('timeCard-id')->startBreak()->post($requestRequestBody);


```