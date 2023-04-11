---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RefRequestBuilderDeleteRequestConfiguration(
)


await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').publishedResources_by_id('publishedResource-id').agentGroups_by_id('onPremisesAgentGroup-id').ref.delete()


```