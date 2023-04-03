---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AgentGroupsRequestBuilderGetRequestConfiguration();

queryParameters = AgentGroupsRequestBuilderGetQueryParameters();
queryParameters.expand = ["agents","publishedResources"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agentGroups().get(requestConfiguration);


```