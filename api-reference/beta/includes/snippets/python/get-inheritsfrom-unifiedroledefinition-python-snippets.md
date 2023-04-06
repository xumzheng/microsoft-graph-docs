---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration(
request_configuration = UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration(query_params=query_params = UnifiedRoleDefinitionRequestBuilderGetQueryParameters()
query_params['expand'] = ["inheritsPermissionsFrom"]

)
query_params = UnifiedRoleDefinitionRequestBuilderGetQueryParameters()
query_params['expand'] = ["inheritsPermissionsFrom"]

)


result = await client.roleManagement.directory.roleDefinitions_by_id('unifiedRoleDefinition-id').get(request_configuration)


```