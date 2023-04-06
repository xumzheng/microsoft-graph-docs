---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnPremisesAgentGroup()
request_body.setDisplayName('Group New Name')


request_config = OnPremisesAgentGroupRequestBuilderPatchRequestConfiguration(
request_config = OnPremisesAgentGroupRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agentGroups_by_id('onPremisesAgentGroup-id').patch(request_body, headers=)


```