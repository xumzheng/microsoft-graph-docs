---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InternalDomainFederation();


$requestRequestBody->setDisplayName('Contoso');
$requestRequestBody->setIssuerUri('http://contoso.com/adfs/services/trust');
$requestRequestBody->setMetadataExchangeUri('https://sts.contoso.com/adfs/services/trust/mex');
$requestRequestBody->setSigningCertificate('MIIE3jCCAsagAwIBAgIQQcyDaZz3MI');
$requestRequestBody->setPassiveSignInUri('https://sts.contoso.com/adfs/ls');
$requestRequestBody->setPreferredAuthenticationProtocol(new AuthenticationProtocol('wsFed'));
$requestRequestBody->setActiveSignInUri('https://sts.contoso.com/adfs/services/trust/2005/usernamemixed');
$requestRequestBody->setSignOutUri('https://sts.contoso.com/adfs/ls');
$requestRequestBody->setPromptLoginBehavior(new PromptLoginBehavior('nativeSupport'));
$requestRequestBody->setIsSignedAuthenticationRequestRequired(True);
$requestRequestBody->setNextSigningCertificate('MIIE3jCCAsagAwIBAgIQQcyDaZz3MI');
$requestRequestBody->setFederatedIdpMfaBehavior(new FederatedIdpMfaBehavior('rejectMfaByFederatedIdp'));
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.internalDomainFederation',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->domainsById('domain-id')->federationConfiguration()->post($requestRequestBody);


```