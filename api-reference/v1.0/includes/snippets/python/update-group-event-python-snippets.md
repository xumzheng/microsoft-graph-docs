---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
location = Location()
location.setDisplayName('Conf Room 2')


request_body.setLocation($location)


result = await client.groupsById('group-id').calendar.eventsById('event-id').patch(request_body)


```