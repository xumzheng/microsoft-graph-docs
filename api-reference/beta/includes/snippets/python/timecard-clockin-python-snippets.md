---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ClockInPostRequestBody();
$notes = new ItemBody();
$notes->setContentType(new BodyType('text'));

$notes->setContent('clock in notes');


$requestBody->setNotes($notes);
$additionalData = [
'atAprovedLocation' => true,
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->teamsById('team-id')->schedule()->timeCards()->clockIn()->post($requestBody);


```