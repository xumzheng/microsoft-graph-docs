---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = HorizontalSectionRequestBuilder.HorizontalSectionRequestBuilderGetQueryParameters(
		select = ["id","expand=columns"],
)

request_configuration = HorizontalSectionRequestBuilder.HorizontalSectionRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').canvasLayout.horizontalSections_by_id('horizontalSection-id').get(request_configuration = request_configuration)


```