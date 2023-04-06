---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ConditionalAccessTemplateRequestBuilderGetRequestConfiguration(
request_configuration = ConditionalAccessTemplateRequestBuilderGetRequestConfiguration(query_params=query_params = ConditionalAccessTemplateRequestBuilderGetQueryParameters()
query_params['select'] = ["details"]

)
query_params = ConditionalAccessTemplateRequestBuilderGetQueryParameters()
query_params['select'] = ["details"]

)


result = await client.identity.conditionalAccess.templates_by_id('conditionalAccessTemplate-id').get(request_configuration)


```