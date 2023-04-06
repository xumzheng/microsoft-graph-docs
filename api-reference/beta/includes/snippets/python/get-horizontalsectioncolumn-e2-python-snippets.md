---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = HorizontalSectionColumnRequestBuilderGetRequestConfiguration(
request_config = HorizontalSectionColumnRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","expand=webparts"]
)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').canvasLayout.horizontalSections_by_id('horizontalSection-id').columns_by_id('horizontalSectionColumn-id').get(request_config, headers=request_config)


```