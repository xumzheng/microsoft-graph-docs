---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RefRequestBuilderDeleteRequestConfiguration(
)


await client.policies.featureRolloutPolicies_by_id('featureRolloutPolicy-id').appliesTo_by_id('directoryObject-id').ref.delete()


```