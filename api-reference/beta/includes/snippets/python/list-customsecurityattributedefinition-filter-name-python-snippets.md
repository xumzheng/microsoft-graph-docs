---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration(
request_config = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "name eq 'Project' and status eq 'Available'"
)


result = await client.directory.customSecurityAttributeDefinitions.get(request_config, headers=request_config)


```