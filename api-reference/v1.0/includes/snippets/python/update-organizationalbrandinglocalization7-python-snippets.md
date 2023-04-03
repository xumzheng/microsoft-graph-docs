---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OrganizationalBrandingLocalization();
requestBody.setSignInPageText('Welcome to Contoso France.');

requestBody.setUsernameHintText(' ');



requestResult = graphServiceClient.organizationById('organization-id').branding().localizationsById('organizationalBrandingLocalization-id').patch(requestBody);


```