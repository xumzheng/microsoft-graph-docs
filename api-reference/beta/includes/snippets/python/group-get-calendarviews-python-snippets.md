---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = CalendarViewRequestBuilderGetRequestConfiguration();

query_params = CalendarViewRequestBuilderGetQueryParameters();
query_params.startDateTime = "2017-01-01T19:00:00-08:00";
query_params.endDateTime = "2017-10-01T19:00:00.00-08:00";

headers = [
'Prefer' => 'outlook.body-content-type="text"',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.groupsById('group-id').calendarView().get(request_config);


```