---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = CalendarViewRequestBuilderGetRequestConfiguration();

query_params = CalendarViewRequestBuilderGetQueryParameters();
query_params.start = "2018-04-30T00:00:00Z";
query_params.end = "2018-05-10T00:00:00Z";

request_config.queryParameters = query_params;


result = awaitclient.solutions().bookingBusinessesById('bookingBusiness-id').calendarView().get(request_config);


```