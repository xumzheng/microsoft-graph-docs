---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CalendarViewRequestBuilderGetRequestConfiguration(
request_config = CalendarViewRequestBuilderGetRequestConfiguration(query_params=params['startDateTime'] = "2020-01-01T19:00:00-08:00"
params['endDateTime'] = "2020-01-02T19:00:00-08:00"
)


result = await client.me.calendarView.get(request_config, headers=request_config)


```