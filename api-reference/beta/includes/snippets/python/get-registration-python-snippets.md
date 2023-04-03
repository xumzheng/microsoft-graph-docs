---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = RegistrationRequestBuilderGetRequestConfiguration();

query_params = RegistrationRequestBuilderGetQueryParameters();
query_params.expand = ["microsoft.graph.meetingRegistration/customQuestions"];

request_config.queryParameters = query_params;


result = awaitclient.me().onlineMeetingsById('onlineMeeting-id').registration().get(request_config);


```