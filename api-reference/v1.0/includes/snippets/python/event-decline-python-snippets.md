---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DeclinePostRequestBody();
requestBody.setComment('I won\'t be able to make this week. How about next week?');

requestBody.setSendResponse(true);

proposedNewTime = TimeSlot();
proposedNewTimeStart = DateTimeTimeZone();
proposedNewTimeStart.setDateTime('2019-12-02T18:00:00');

proposedNewTimeStart.setTimeZone('Pacific Standard Time');


proposedNewTime.setStart($proposedNewTimeStart);
proposedNewTimeEnd = DateTimeTimeZone();
proposedNewTimeEnd.setDateTime('2019-12-02T19:00:00');

proposedNewTimeEnd.setTimeZone('Pacific Standard Time');


proposedNewTime.setEnd($proposedNewTimeEnd);

requestBody.setProposedNewTime($proposedNewTime);


await client.me().eventsById('event-id').decline().post(requestBody);


```