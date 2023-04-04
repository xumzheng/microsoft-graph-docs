---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = StartBreakPostRequestBody();
notes = ItemBody();
notes.setContentType(BodyType('text'));

notes.setContent('start break smaple notes');


request_body.setNotes($notes);
additionalData = [
'atAprovedLocation' => true,
];
request_body.setAdditionalData(additionalData);




result = await client.teamsById('team-id').schedule().timeCardsById('timeCard-id').startBreak().post(request_body);


```