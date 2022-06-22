---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new B2xIdentityUserFlow();


$requestRequestBody->setId('UserFlowWithAPIConnector');
$requestRequestBody->setUserFlowType(new UserFlowType('signUpOrSignIn'));
$requestRequestBody->setUserFlowTypeVersion(1);

$apiConnectorConfiguration = new UserFlowApiConnectorConfiguration();
$requestRequestBody->setApiConnectorConfiguration($apiConnectorConfiguration);



$postFederationSignup = new IdentityApiConnector();
$apiConnectorConfiguration->setPostFederationSignup($postFederationSignup);


$postFederationSignupAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}',
];
$postFederationSignup->setAdditionalData($postFederationSignupAdditionalData);


$postAttributeCollection = new IdentityApiConnector();
$apiConnectorConfiguration->setPostAttributeCollection($postAttributeCollection);


$postAttributeCollectionAdditionalData = [
"@odata.id" => 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}',
];
$postAttributeCollection->setAdditionalData($postAttributeCollectionAdditionalData);


$result =  $graphClient->identity()->b2xUserFlows()->post($requestRequestBody);


```