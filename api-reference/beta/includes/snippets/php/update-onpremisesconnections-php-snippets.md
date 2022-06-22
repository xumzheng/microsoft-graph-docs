---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcOnPremisesConnection();


$requestRequestBody->setDisplayName('Display Name value');
$requestRequestBody->setSubscriptionId('0ac520ee-14c0-480f-b6c9-0a90c585ffff');
$requestRequestBody->setSubscriptionName('Subscription Name value');
$requestRequestBody->setAdDomainName('Active Directory Domain Name value');
$requestRequestBody->setAdDomainUsername('Active Directory Domain User Name value');
$requestRequestBody->setOrganizationalUnit('Organization Unit value');
$requestRequestBody->setResourceGroupId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG');
$requestRequestBody->setVirtualNetworkId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet');
$requestRequestBody->setSubnetId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.cloudPcOnPremisesConnection',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->onPremisesConnectionsById('cloudPcOnPremisesConnection-id')->patch($requestRequestBody);


```