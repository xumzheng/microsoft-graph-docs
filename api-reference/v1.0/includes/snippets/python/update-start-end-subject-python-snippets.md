---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnlineMeeting()
request_body.setStartDateTime(DateTime('2020-09-09T14:33:30.8546353-07:00'))

request_body.setEndDateTime(DateTime('2020-09-09T15:03:30.8566356-07:00'))

request_body.setSubject('Patch Meeting Subject')



result = await client.me.onlineMeetings._by_id('onlineMeeting-id').patch(request_body)


```