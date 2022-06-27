---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthenticationMethodConfiguration();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.emailAuthenticationMethodConfiguration',
	"allowExternalIdToUseEmailOtp" => 'disabled',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->policies()->authenticationMethodsPolicy()->authenticationMethodConfigurationsById('authenticationMethodConfiguration-id')->patch($requestRequestBody);


```