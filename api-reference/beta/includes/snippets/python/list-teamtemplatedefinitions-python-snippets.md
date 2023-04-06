---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamTemplatesRequestBuilderGetRequestConfiguration(
request_configuration = TeamTemplatesRequestBuilderGetRequestConfiguration(query_params=query_params = TeamTemplatesRequestBuilderGetQueryParameters()
query_params['expand'] = ["definitions"]
query_params['filter'] = "definitions/any"

)
query_params = TeamTemplatesRequestBuilderGetQueryParameters()
query_params['expand'] = ["definitions"]
query_params['filter'] = "definitions/any"

)


result = await client.teamwork.teamTemplates.get(request_configuration)


```