---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OrganizationalBrandingLocalization();
$requestBody->setBackgroundColor('#00000F');

$requestBody->setId('fr-FR');

$requestBody->setSignInPageText(' ');



$requestResult = $graphServiceClient->organizationById('organization-id')->branding()->localizations()->post($requestBody);


```