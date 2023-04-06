---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration(
request_config = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'"
)


result = await client.directory.customSecurityAttributeDefinitions.get(request_config, headers=request_config)


```