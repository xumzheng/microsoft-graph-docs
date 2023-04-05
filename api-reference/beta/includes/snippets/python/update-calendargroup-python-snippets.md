---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarGroup()
request_body.setName('name-value')



result = await client.me_calendarGroupsby_id('calendarGroup-id').patch(request_body)


```