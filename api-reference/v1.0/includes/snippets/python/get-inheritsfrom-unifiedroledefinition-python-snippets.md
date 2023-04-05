---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration()

query_params = UnifiedRoleDefinitionRequestBuilderGetQueryParameters()
query_params.expand = ["inheritsPermissionsFrom"]

request_config.queryParameters = query_params


result = await client.roleManagement.directory.roleDefinitionsby_id('unifiedRoleDefinition-id').get(request_config)


```