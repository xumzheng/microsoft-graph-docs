---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = DeltaRequestBuilderGetRequestConfiguration()

query_params = DeltaRequestBuilderGetQueryParameters()
query_params.token = "1230919asd190410jlka"

request_config.queryParameters = query_params


result = await client.sitesById('site-id').listsById('list-id').items.delta.get(request_config)


```