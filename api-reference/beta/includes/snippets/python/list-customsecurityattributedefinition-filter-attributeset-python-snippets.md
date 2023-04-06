---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration(
request_configuration = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration(query_params=query_params = CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters()
query_params['filter'] = "attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'"

)
query_params = CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters()
query_params['filter'] = "attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'"

)


result = await client.directory.customSecurityAttributeDefinitions.get(request_configuration)


```