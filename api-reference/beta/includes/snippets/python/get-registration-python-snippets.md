---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RegistrationRequestBuilderGetRequestConfiguration();

queryParameters = RegistrationRequestBuilderGetQueryParameters();
queryParameters.expand = ["microsoft.graph.meetingRegistration/customQuestions"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().onlineMeetingsById('onlineMeeting-id').registration().get(requestConfiguration);


```