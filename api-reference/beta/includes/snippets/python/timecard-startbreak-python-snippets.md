---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = StartBreakPostRequestBody();
notes = ItemBody();
notes.setContentType(BodyType('text'));

notes.setContent('start break smaple notes');


requestBody.setNotes($notes);
additionalData = [
'atAprovedLocation' => true,
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.teamsById('team-id').schedule().timeCardsById('timeCard-id').startBreak().post(requestBody);


```