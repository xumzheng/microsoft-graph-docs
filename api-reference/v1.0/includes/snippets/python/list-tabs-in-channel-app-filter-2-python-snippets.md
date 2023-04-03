---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TabsRequestBuilderGetRequestConfiguration();

queryParameters = TabsRequestBuilderGetQueryParameters();
queryParameters.expand = ["teamsApp"];
queryParameters.filter = "teamsApp/id eq 'com.microsoft.teamspace.tab.planner'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').channelsById('channel-id').tabs().get(requestConfiguration);


```