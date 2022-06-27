---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OrganizationalBranding();


$requestRequestBody->setSignInPageText('Default');
$requestRequestBody->setUsernameHintText('DefaultHint');
$requestConfiguration = new BrandingRequestBuilderPatchRequestConfiguration();

$headers = [
"Accept-Language" => "0",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->organizationById('organization-id')->branding()->patch($requestRequestBody, $requestConfiguration);


```