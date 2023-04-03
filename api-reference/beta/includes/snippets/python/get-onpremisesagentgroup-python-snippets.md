---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = OnPremisesAgentGroupRequestBuilderGetRequestConfiguration();

queryParameters = OnPremisesAgentGroupRequestBuilderGetQueryParameters();
queryParameters.expand = ["publishedResources","agents"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agentGroupsById('onPremisesAgentGroup-id').get(requestConfiguration);


```