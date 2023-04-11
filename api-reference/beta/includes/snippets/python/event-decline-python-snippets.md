---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeclinePostRequestBody()
request_body.comment = 'I won\'t be able to make this week. How about next week?'

request_body.sendResponse = true

proposedNewTime = TimeSlot()
proposedNewTimeStart = DateTimeTimeZone()
proposedNewTimeStart.dateTime = '2019-12-02T18:00:00'

proposedNewTimeStart.timeZone = 'Pacific Standard Time'


proposedNewTime.start = proposedNewTimeStart
proposedNewTimeEnd = DateTimeTimeZone()
proposedNewTimeEnd.dateTime = '2019-12-02T19:00:00'

proposedNewTimeEnd.timeZone = 'Pacific Standard Time'


proposedNewTime.end = proposedNewTimeEnd

request_body.proposedNewTime = proposedNewTime


request_configuration = DeclineRequestBuilderPostRequestConfiguration(
)


await client.me.events_by_id('event-id').decline.post(request_body = request_body)


```