---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = BrandingRequestBuilderGetRequestConfiguration()

headers = [
	'Accept-Language' => '0',
]

request_config.headers = headers


result = await client.organizationById('organization-id').branding.get(request_config)


```