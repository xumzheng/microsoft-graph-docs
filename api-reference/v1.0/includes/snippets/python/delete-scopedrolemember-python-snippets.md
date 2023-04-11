---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = ScopedRoleMembershipRequestBuilderDeleteRequestConfiguration(
)


await client.directory.administrativeUnits_by_id('administrativeUnit-id').scopedRoleMembers_by_id('scopedRoleMembership-id').delete()


```