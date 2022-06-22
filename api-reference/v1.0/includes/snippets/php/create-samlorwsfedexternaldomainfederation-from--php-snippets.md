---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProviderBase();


$requestRequestBody->setDisplayName('contoso display name');
$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.samlOrWsFedExternalDomainFederation',
	"issuerUri" => 'https://contoso.com/issuerUri',
	"metadataExchangeUri" => 'https://contoso.com/metadataExchangeUri',
	"passiveSignInUri" => 'https://contoso.com/signin',
	"preferredAuthenticationProtocol" => 'wsFed',
	"domains" =>  [
	],
	"signingCertificate" => 'MIIDADCCAeigAwIBAgIQEX41y8r6',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->directory()->federationConfigurations()->post($requestRequestBody);


```