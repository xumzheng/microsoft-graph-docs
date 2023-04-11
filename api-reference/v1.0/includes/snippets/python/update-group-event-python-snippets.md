---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
location = Location()
location.displayName = 'Conf Room 2'


request_body.location = location



result = await client.groups_by_id('group-id').calendar.events_by_id('event-id').patch(request_body = request_body)


```