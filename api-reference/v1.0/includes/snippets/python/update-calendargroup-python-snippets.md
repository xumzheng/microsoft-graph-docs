---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarGroup()
request_body.name = 'name-value'



request_configuration = CalendarGroupRequestBuilderPatchRequestConfiguration(
)


result = await client.me.calendarGroups_by_id('calendarGroup-id').patch(request_body = request_body)


```