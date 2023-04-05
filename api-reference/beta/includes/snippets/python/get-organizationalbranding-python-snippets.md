---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = BrandingRequestBuilderGetRequestConfiguration(
headers = [
	'Accept-Language' => '0',
]

)


result = await client.organization_by_id('organization-id').branding.get(request_config)


```