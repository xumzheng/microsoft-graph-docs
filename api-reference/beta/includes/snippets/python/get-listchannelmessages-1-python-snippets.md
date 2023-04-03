---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessagesRequestBuilderGetRequestConfiguration();

queryParameters = MessagesRequestBuilderGetQueryParameters();
queryParameters.top = 3;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').channelsById('channel-id').messages().get(requestConfiguration);


```