---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OrganizationalBrandingLocalization();


$requestRequestBody->setBackgroundColor('#00000F');
$requestRequestBody->setId('fr-FR');
$requestRequestBody->setSignInPageText(' ');
$result =  $graphClient->organizationById('organization-id')->branding()->localizations()->post($requestRequestBody);


```