---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = CalendarViewRequestBuilderGetRequestConfiguration();

query_params = CalendarViewRequestBuilderGetQueryParameters();
query_params.startDateTime = "2020-01-01T19:00:00-08:00";
query_params.endDateTime = "2020-01-02T19:00:00-08:00";

request_config.queryParameters = query_params;


result = awaitclient.me().calendarView().get(request_config);


```