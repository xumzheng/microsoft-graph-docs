---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OrganizationalBranding();
$requestBody->setSignInPageText('Default');

$requestBody->setUsernameHintText('DefaultHint');


$requestConfiguration = new BrandingRequestBuilderPatchRequestConfiguration();

$headers = [
	'Accept-Language' => '0',
];

$requestConfiguration->headers = $headers;


$requestResult = $graphServiceClient->organizationById('organization-id')->branding()->patch($requestBody, $requestConfiguration);


```