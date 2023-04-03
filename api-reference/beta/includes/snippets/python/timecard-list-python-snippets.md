---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TimeCardsRequestBuilderGetRequestConfiguration();

queryParameters = TimeCardsRequestBuilderGetQueryParameters();
queryParameters.top = 2;
queryParameters.filter = "state eq 'clockedOut'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').schedule().timeCards().get(requestConfiguration);


```