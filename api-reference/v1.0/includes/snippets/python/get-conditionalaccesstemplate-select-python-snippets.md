---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ConditionalAccessTemplateRequestBuilderGetRequestConfiguration()

query_params = ConditionalAccessTemplateRequestBuilderGetQueryParameters()
query_params.select = ["details"]

request_config.queryParameters = query_params


result = await client.identity_conditionalAccess_templatesby_id('conditionalAccessTemplate-id').get(request_config)


```