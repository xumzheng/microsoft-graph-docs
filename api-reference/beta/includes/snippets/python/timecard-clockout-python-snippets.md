---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClockOutPostRequestBody()
notes = ItemBody()
notes.setContentType(BodyType('text'))

notes.setContent('clock out smaple notes')


request_body.setNotes($notes)
additionalData = [
'atAprovedLocation' => true,
];
request_body.setAdditionalData(additionalData)




result = await client.teams_by_id('team-id').schedule.timeCards_by_id('timeCard-id').clockOut.post(request_body)


```