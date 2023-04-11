---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TeamTemplatesRequestBuilder.TeamTemplatesRequestBuilderGetQueryParameters(
		expand = ["definitions"],
		filter = "definitions/any",
)

request_configuration = TeamTemplatesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.teamwork.teamTemplates.get(request_configuration = request_configuration)


```