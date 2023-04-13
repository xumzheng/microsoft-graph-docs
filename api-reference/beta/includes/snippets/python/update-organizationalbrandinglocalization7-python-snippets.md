---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OrganizationalBrandingLocalization()
request_body.signInPageText = 'Welcome to Contoso France.'

request_body.usernameHintText = ' '




result = await client.organization_by_id('organization-id').branding.localizations_by_id('organizationalBrandingLocalization-id').patch(request_body = request_body)


```