---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = EventRequestBuilderGetRequestConfiguration();

queryParameters = EventRequestBuilderGetQueryParameters();
queryParameters.select = ["isOnlineMeeting","onlineMeetingProvider","onlineMeeting"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().eventsById('event-id').get(requestConfiguration);


```