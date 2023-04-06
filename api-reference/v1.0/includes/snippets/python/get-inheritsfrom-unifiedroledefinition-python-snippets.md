---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration(
request_config = UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration(query_params=query_params = UnifiedRoleDefinitionRequestBuilderGetQueryParameters()
query_params.expand = ["inheritsPermissionsFrom"]

)
query_params = UnifiedRoleDefinitionRequestBuilderGetQueryParameters()
query_params.expand = ["inheritsPermissionsFrom"]

)


result = await client.roleManagement.directory.roleDefinitions_by_id('unifiedRoleDefinition-id').get(request_config, headers=request_config)


```