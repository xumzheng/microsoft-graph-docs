---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = BrandingRequestBuilderGetRequestConfiguration()

headers = [
	'Accept-Language' => 'fr-FR',
]

request_config.headers = headers


result = await client.organization._by_id('organization-id').branding.get(request_config)


```