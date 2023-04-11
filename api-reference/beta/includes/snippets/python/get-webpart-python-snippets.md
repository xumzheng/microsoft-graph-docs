---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = WebPartRequestBuilderGetRequestConfiguration(
)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').webParts_by_id('webPart-id').get()


```