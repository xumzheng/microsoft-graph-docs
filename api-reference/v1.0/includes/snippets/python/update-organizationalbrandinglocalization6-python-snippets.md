---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OrganizationalBrandingLocalization();
requestBody.setBackgroundColor('#00000F');

requestBody.setSignInPageText('Welcome to Contoso France');



result = await client.organizationById('organization-id').branding().localizationsById('organizationalBrandingLocalization-id').patch(requestBody);


```