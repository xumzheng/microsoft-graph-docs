---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DeltaRequestBuilderGetRequestConfiguration();

queryParameters = DeltaRequestBuilderGetQueryParameters();
queryParameters.top = 2;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').channelsById('channel-id').messages().delta().get(requestConfiguration);


```