---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = CalendarViewRequestBuilderGetRequestConfiguration(
request_configuration = CalendarViewRequestBuilderGetRequestConfiguration(query_params=query_params = CalendarViewRequestBuilderGetQueryParameters()
query_params['startDateTime'] = "2017-01-01T19:00:00-08:00"
query_params['endDateTime'] = "2017-10-01T19:00:00.00-08:00"

)
query_params = CalendarViewRequestBuilderGetQueryParameters()
query_params['startDateTime'] = "2017-01-01T19:00:00-08:00"
query_params['endDateTime'] = "2017-10-01T19:00:00.00-08:00"

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups_by_id('group-id').calendarView.get(request_configuration)


```