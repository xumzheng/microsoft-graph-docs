---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProviderBase();


$requestRequestBody->setDisplayName('Login with the Contoso identity provider');
$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.openIdConnectIdentityProvider',
	"clientId" => '56433757-cadd-4135-8431-2c9e3fd68ae8',
	"clientSecret" => '12345',
	"domainHint" => 'mycustomoidc',
	"metadataUrl" => 'https://mycustomoidc.com/.well-known/openid-configuration',
	"responseMode" => 'form_post',
	"responseType" => 'code',
	"scope" => 'openid',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->identityProviders()->post($requestRequestBody);


```