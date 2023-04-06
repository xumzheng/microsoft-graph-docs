---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = HorizontalSectionRequestBuilderGetRequestConfiguration(
request_configuration = HorizontalSectionRequestBuilderGetRequestConfiguration(query_params=query_params = HorizontalSectionRequestBuilderGetQueryParameters()
query_params['select'] = ["id","expand=columns"]

)
query_params = HorizontalSectionRequestBuilderGetQueryParameters()
query_params['select'] = ["id","expand=columns"]

)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').canvasLayout.horizontalSections_by_id('horizontalSection-id').get(request_configuration)


```