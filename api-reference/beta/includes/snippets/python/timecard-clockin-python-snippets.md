---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClockInPostRequestBody()
notes = ItemBody()
notes.setContentType(BodyType('text'))

notes.setContent('clock in notes')


request_body.setNotes($notes)
additionalData = [
'atAprovedLocation' => true,
];
request_body.setAdditionalData(additionalData)




result = await client.teamsby_id('team-id')_schedule_timeCards_clockIn.post(request_body)


```