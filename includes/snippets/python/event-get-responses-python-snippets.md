---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = EventRequestBuilderGetRequestConfiguration(
)


result = await client.me.calendar.events_by_id('event-id').get()


```