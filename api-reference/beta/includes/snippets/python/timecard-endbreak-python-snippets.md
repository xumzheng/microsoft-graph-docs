---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EndBreakPostRequestBody();
$notes = new ItemBody();
$notes->setContentType(new BodyType('text'));

$notes->setContent('end break smaple notes');


$requestBody->setNotes($notes);
$additionalData = [
'atAprovedLocation' => true,
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->teamsById('team-id')->schedule()->timeCardsById('timeCard-id')->endBreak()->post($requestBody);


```