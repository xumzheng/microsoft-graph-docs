---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = CalendarViewRequestBuilderGetRequestConfiguration();

queryParameters = CalendarViewRequestBuilderGetQueryParameters();
queryParameters.startDateTime = "2017-01-01T19:00:00-08:00";
queryParameters.endDateTime = "2017-10-01T19:00:00.00-08:00";

headers = [
'Prefer' => 'outlook.body-content-type="text"',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.groupsById('group-id').calendarView().get(requestConfiguration);


```