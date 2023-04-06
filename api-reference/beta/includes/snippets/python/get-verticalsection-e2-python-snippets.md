---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = VerticalSectionRequestBuilderGetRequestConfiguration(
request_configuration = VerticalSectionRequestBuilderGetRequestConfiguration(query_params=query_params = VerticalSectionRequestBuilderGetQueryParameters()
query_params['select'] = ["emphasis","expand=webparts"]

)
query_params = VerticalSectionRequestBuilderGetQueryParameters()
query_params['select'] = ["emphasis","expand=webparts"]

)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').canvasLayout.verticalSection.get(request_configuration)


```