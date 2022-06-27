---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConnectedOrganization();


$requestRequestBody->setDisplayName('Connected organization name');
$requestRequestBody->setDescription('Connected organization description');
$identitySourcesArray = [];

$identitySourcesidentitySources1 = new IdentitySource();

$identitySourcesidentitySources1AdditionalData = [
	"@odata.type" => '#microsoft.graph.domainIdentitySource',
	"domainName" => 'example.com',
	"displayName" => 'example.com',
];
$identitySourcesidentitySources1->setAdditionalData($identitySourcesidentitySources1AdditionalData);

$identitySourcesArray []= $identitySourcesidentitySources1;
$requestRequestBody->setIdentitySources($identitySourcesArray);
$requestRequestBody->setState(new ConnectedOrganizationState('proposed'));
$result =  $graphClient->identityGovernance()->entitlementManagement()->connectedOrganizations()->post($requestRequestBody);


```