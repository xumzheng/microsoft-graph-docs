---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TemplatesRequestBuilderGetRequestConfiguration(
request_configuration = TemplatesRequestBuilderGetRequestConfiguration(query_params=query_params = TemplatesRequestBuilderGetQueryParameters()
query_params['select'] = ["name","description","id","scenarios"]
query_params['filter'] = "scenarios has 'secureFoundation'"

)
query_params = TemplatesRequestBuilderGetQueryParameters()
query_params['select'] = ["name","description","id","scenarios"]
query_params['filter'] = "scenarios has 'secureFoundation'"

)


result = await client.identity.conditionalAccess.templates.get(request_configuration)


```