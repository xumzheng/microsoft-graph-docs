---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OrganizationalBranding()
request_body.signInPageText = 'Default'

request_body.usernameHintText = 'DefaultHint'



request_configuration = BrandingRequestBuilderPatchRequestConfiguration(
headers = {
					'Accept-Language' : "0",
}

)


result = await client.organization_by_id('organization-id').branding.patch(request_body = request_body, request_configuration = request_configuration)


```