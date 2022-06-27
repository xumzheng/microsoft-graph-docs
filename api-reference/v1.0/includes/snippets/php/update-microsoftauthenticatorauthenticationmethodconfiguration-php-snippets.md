---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthenticationMethodConfiguration();


$requestRequestBody->setState(new AuthenticationMethodState('String'));
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->policies()->authenticationMethodsPolicy()->authenticationMethodConfigurationsById('authenticationMethodConfiguration-id')->patch($requestRequestBody);


```