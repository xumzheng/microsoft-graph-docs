---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration(
request_configuration = UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration(query_params=query_params = UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters()
query_params['expand'] = ["roleDefinition","principals","directoryScopes"]

)
query_params = UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters()
query_params['expand'] = ["roleDefinition","principals","directoryScopes"]

)


result = await client.roleManagement.deviceManagement.roleAssignments_by_id('unifiedRoleAssignmentMultiple-id').get(request_configuration)


```