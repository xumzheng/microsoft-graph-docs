---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeclinePostRequestBody()
request_body.setComment('I won\'t be able to make this week. How about next week?')

request_body.setSendResponse(true)

proposedNewTime = TimeSlot()
proposedNewTimeStart = DateTimeTimeZone()
proposedNewTimeStart.setDateTime('2019-12-02T18:00:00')

proposedNewTimeStart.setTimeZone('Pacific Standard Time')


proposedNewTime.setStart($proposedNewTimeStart)
proposedNewTimeEnd = DateTimeTimeZone()
proposedNewTimeEnd.setDateTime('2019-12-02T19:00:00')

proposedNewTimeEnd.setTimeZone('Pacific Standard Time')


proposedNewTime.setEnd($proposedNewTimeEnd)

request_body.setProposedNewTime($proposedNewTime)

request_config = DeclineRequestBuilderPostRequestConfiguration(
request_config = DeclineRequestBuilderPostRequestConfiguration(query_params=)


await client.me.events_by_id('event-id').decline.post(request_body, headers=)


```