---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration();

queryParameters = OnPremisesPublishingProfileRequestBuilderGetQueryParameters();
queryParameters.expand = ["publishedResources","agents","agentGroups"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').get(requestConfiguration);


```