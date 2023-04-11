---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EndBreakPostRequestBody()
notes = ItemBody()
notes.ContentType(BodyType('text'))

notes.content = 'end break smaple notes'


request_body.notes = notes
additionalData = [
'atAprovedLocation' => true,
];
request_body.additionaldata(additionalData)




request_configuration = EndBreakRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').schedule.timeCards_by_id('timeCard-id').endBreak.post(request_body = request_body)


```