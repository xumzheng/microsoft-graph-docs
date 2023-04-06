---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TemplatesRequestBuilderGetRequestConfiguration(
request_config = TemplatesRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["name","description","id","scenarios"]
params['filter'] = "scenarios has 'secureFoundation'"
)


result = await client.identity.conditionalAccess.templates.get(request_config, headers=request_config)


```