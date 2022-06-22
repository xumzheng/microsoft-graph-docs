---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new BrandingRequestBuilderGetRequestConfiguration();

$headers = [
	"Accept-Language" => "fr-FR",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->organizationById('organization-id')->branding()->get($requestConfiguration);


```