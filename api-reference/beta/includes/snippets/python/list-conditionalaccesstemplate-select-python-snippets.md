---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = TemplatesRequestBuilderGetRequestConfiguration();

query_params = TemplatesRequestBuilderGetQueryParameters;
query_params.select = ["name","description","id","scenarios"];
query_params.filter = "scenarios has 'secureFoundation'";

request_config.queryParameters = query_params;


result = await client.identity().conditionalAccess().templates().get(request_config);


```