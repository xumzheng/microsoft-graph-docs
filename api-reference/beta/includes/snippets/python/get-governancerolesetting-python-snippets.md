---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = GovernanceRoleSettingRequestBuilderGetRequestConfiguration(
)


result = await client.privilegedAccess_by_id('privilegedAccess-id').roleSettings_by_id('governanceRoleSetting-id').get()


```