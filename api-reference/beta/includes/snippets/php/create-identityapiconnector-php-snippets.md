---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityApiConnector();


$requestRequestBody->setDisplayName('Test API');
$requestRequestBody->setTargetUrl('https://someotherapi.com/api');

$authenticationConfiguration = new ApiAuthenticationConfigurationBase();
$requestRequestBody->setAuthenticationConfiguration($authenticationConfiguration);


$authenticationConfigurationAdditionalData = [
	"@odata.type" => '#microsoft.graph.pkcs12Certificate',
	"pkcs12Value" => 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA',
	"password" => '<password>',
];
$authenticationConfiguration->setAdditionalData($authenticationConfigurationAdditionalData);

$result =  $graphClient->identity()->apiConnectors()->post($requestRequestBody);


```