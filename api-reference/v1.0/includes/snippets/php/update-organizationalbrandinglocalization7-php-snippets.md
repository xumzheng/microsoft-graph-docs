---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OrganizationalBrandingLocalization();


$requestRequestBody->setSignInPageText('Welcome to Contoso France.');
$requestRequestBody->setUsernameHintText(' ');
$result =  $graphClient->organizationById('organization-id')->branding()->localizationsById('organizationalBrandingLocalization-id')->patch($requestRequestBody);


```