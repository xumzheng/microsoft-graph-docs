---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CalendarViewRequestBuilderGetRequestConfiguration(
request_config = CalendarViewRequestBuilderGetRequestConfiguration(query_params=query_params = CalendarViewRequestBuilderGetQueryParameters()
query_params.start = "2018-04-30T00:00:00Z"
query_params.end = "2018-05-10T00:00:00Z"

)
query_params = CalendarViewRequestBuilderGetQueryParameters()
query_params.start = "2018-04-30T00:00:00Z"
query_params.end = "2018-05-10T00:00:00Z"

)


result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').calendarView.get(request_config, headers=request_config)


```