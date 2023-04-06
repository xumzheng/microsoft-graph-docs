---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = StartBreakPostRequestBody()
notes = ItemBody()
notes.setContentType(BodyType('text'))

notes.setContent('start break smaple notes')


request_body.setNotes($notes)
additionalData = [
'atAprovedLocation' => true,
];
request_body.setAdditionalData(additionalData)



request_config = StartBreakRequestBuilderPostRequestConfiguration(
request_config = StartBreakRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').schedule.timeCards_by_id('timeCard-id').startBreak.post(request_body, headers=)


```