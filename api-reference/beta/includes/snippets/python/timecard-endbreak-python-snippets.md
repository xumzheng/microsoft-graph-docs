---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EndBreakPostRequestBody()
notes = ItemBody()
notes.setContentType(BodyType('text'))

notes.setContent('end break smaple notes')


request_body.setNotes($notes)
additionalData = [
'atAprovedLocation' => true,
];
request_body.setAdditionalData(additionalData)




result = await client.teamsby_id('team-id')_schedule_timeCardsby_id('timeCard-id')_endBreak.post(request_body)


```