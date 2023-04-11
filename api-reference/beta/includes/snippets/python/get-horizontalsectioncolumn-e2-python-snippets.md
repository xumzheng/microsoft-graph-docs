---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = HorizontalSectionColumnRequestBuilder.HorizontalSectionColumnRequestBuilderGetQueryParameters(
		select = ["id","expand=webparts"],
)

request_configuration = HorizontalSectionColumnRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').canvasLayout.horizontalSections_by_id('horizontalSection-id').columns_by_id('horizontalSectionColumn-id').get(request_configuration = request_configuration)


```