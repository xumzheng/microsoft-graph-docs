---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RefRequestBuilderDeleteRequestConfiguration(
)


await client.policies.mobileDeviceManagementPolicies_by_id('mobilityManagementPolicy-id').includedGroups_by_id('group-id').ref.delete()


```