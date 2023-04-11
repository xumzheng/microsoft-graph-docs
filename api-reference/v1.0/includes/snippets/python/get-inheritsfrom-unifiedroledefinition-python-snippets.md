---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UnifiedRoleDefinitionRequestBuilder.UnifiedRoleDefinitionRequestBuilderGetQueryParameters(
		expand = ["inheritsPermissionsFrom"],
)

request_configuration = UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.roleManagement.directory.roleDefinitions_by_id('unifiedRoleDefinition-id').get(request_configuration = request_configuration)


```