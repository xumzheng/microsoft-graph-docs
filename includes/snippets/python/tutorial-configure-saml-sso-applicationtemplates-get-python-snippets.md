---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ApplicationTemplatesRequestBuilderGetRequestConfiguration(
request_configuration = ApplicationTemplatesRequestBuilderGetRequestConfiguration(query_params=query_params = ApplicationTemplatesRequestBuilderGetQueryParameters()
query_params['filter'] = "displayName eq 'AWS IAM Identity Center '"

)
query_params = ApplicationTemplatesRequestBuilderGetQueryParameters()
query_params['filter'] = "displayName eq 'AWS IAM Identity Center '"

)


result = await client.applicationTemplates.get(request_configuration)


```