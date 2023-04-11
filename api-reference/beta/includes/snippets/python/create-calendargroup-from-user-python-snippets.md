---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarGroup()
request_body.name = 'Personal events'




result = await client.me.calendarGroups.post(request_body = request_body)


```