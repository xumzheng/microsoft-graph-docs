---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EndBreakPostRequestBody();
notes = ItemBody();
notes.setContentType(BodyType('text'));

notes.setContent('end break smaple notes');


requestBody.setNotes($notes);
additionalData = [
'atAprovedLocation' => true,
];
requestBody.setAdditionalData(additionalData);




result = await client.teamsById('team-id').schedule().timeCardsById('timeCard-id').endBreak().post(requestBody);


```