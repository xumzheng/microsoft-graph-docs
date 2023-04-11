---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = HorizontalSectionRequestBuilderGetRequestConfiguration(
)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').canvasLayout.horizontalSections_by_id('horizontalSection-id').get()


```