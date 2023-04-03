---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ClockOutPostRequestBody();
notes = ItemBody();
notes.setContentType(BodyType('text'));

notes.setContent('clock out smaple notes');


requestBody.setNotes($notes);
additionalData = [
'atAprovedLocation' => true,
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.teamsById('team-id').schedule().timeCardsById('timeCard-id').clockOut().post(requestBody);


```