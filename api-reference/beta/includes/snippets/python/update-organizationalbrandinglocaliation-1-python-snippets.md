---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OrganizationalBranding()
request_body.setSignInPageText('Default')

request_body.setUsernameHintText('DefaultHint')


request_config = BrandingRequestBuilderPatchRequestConfiguration(
headers = [
	'Accept-Language' => '0',
]

)


result = await client.organization_by_id('organization-id').branding.patch(request_body, request_config)


```