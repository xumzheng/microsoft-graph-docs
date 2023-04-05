---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration()

query_params = UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters()
query_params.expand = ["roleDefinition","principals","directoryScopes"]

request_config.queryParameters = query_params


result = await client.roleManagement.deviceManagement.roleAssignments._by_id('unifiedRoleAssignmentMultiple-id').get(request_config)


```