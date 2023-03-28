---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OrganizationalBrandingLocalization();
$requestBody.setBackgroundColor('#00000F');

$requestBody.setSignInPageText('Welcome to Contoso France');



$requestResult = $graphServiceClient.organizationById('organization-id').branding().localizationsById('organizationalBrandingLocalization-id').patch($requestBody);


```