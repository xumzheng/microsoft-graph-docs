---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = CalendarViewRequestBuilder.CalendarViewRequestBuilderGetQueryParameters(
		start = "2018-04-30T00:00:00Z",
		end = "2018-05-10T00:00:00Z",
)

request_configuration = CalendarViewRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.bookingBusinesses_by_id('bookingBusiness-id').calendarView.get(request_configuration = request_configuration)


```