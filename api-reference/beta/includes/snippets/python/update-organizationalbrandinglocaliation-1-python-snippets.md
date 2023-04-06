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
request_config = BrandingRequestBuilderPatchRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.organization_by_id('organization-id').branding.patch(request_body, request_config, headers=request_config)


```