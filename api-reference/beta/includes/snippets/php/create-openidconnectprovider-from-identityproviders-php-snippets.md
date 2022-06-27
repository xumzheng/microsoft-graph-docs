---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProvider();


$requestRequestBody->setName('Login with the Contoso identity provider');
$requestRequestBody->setType('OpenIDConnect');
$requestRequestBody->setClientId('56433757-cadd-4135-8431-2c9e3fd68ae8');
$requestRequestBody->setClientSecret('12345');
$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.openIdConnectProvider',
	"domainHint" => 'mycustomoidc',
	"metadataUrl" => 'https://mycustomoidc.com/.well-known/openid-configuration',
	"responseMode" => 'form_post',
	"responseType" => 'code',
	"scope" => 'openid',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityProviders()->post($requestRequestBody);


```