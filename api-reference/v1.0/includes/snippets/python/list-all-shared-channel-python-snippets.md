---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AllChannelsRequestBuilderGetRequestConfiguration();

queryParameters = AllChannelsRequestBuilderGetQueryParameters();
queryParameters.filter = "membershipType eq 'shared'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').allChannels().get(requestConfiguration);


```