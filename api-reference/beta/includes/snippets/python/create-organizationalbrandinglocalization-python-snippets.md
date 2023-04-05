---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OrganizationalBrandingLocalization()
request_body.setBackgroundColor('#00000F')

request_body.setId('fr-FR')

request_body.setSignInPageText(' ')



result = await client.organizationby_id('organization-id').branding.localizations.post(request_body)


```