---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OrganizationalBrandingLocalization()
request_body.setBackgroundColor('#00000F')

request_body.setSignInPageText('Welcome to Contoso France')



result = await client.organization_by_id('organization-id').branding.localizations_by_id('organizationalBrandingLocalization-id').patch(request_body, headers=)


```