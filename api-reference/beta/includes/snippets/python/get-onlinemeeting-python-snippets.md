---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = OnlineMeetingsRequestBuilderGetRequestConfiguration();

queryParameters = OnlineMeetingsRequestBuilderGetQueryParameters();
queryParameters.filter = "VideoTeleconferenceId eq '123456789'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.communications().onlineMeetings().get(requestConfiguration);


```