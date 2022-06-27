---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OrganizationalBrandingLocalization();


$requestRequestBody->setBackgroundColor('#00000F');
$requestRequestBody->setSignInPageText('Welcome to Contoso France');
$result =  $graphClient->organizationById('organization-id')->branding()->localizationsById('organizationalBrandingLocalization-id')->patch($requestRequestBody);


```