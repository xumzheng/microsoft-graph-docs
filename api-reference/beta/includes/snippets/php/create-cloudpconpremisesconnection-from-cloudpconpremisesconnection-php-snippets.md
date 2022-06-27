---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcOnPremisesConnection();


$requestRequestBody->setDisplayName('test-canary-02');
$requestRequestBody->setType(new CloudPcOnPremisesConnectionType('hybridAzureADJoin'));
$requestRequestBody->setSubscriptionId('0ac520ee-14c0-480f-b6c9-0a90c585ffff');
$requestRequestBody->setSubscriptionName('CPC customer 001 test subscription');
$requestRequestBody->setAdDomainName('contoso001.com');
$requestRequestBody->setAdDomainUsername('dcadmin');
$requestRequestBody->setOrganizationalUnit('OU=Domain Controllers, DC=contoso001, DC=com');
$requestRequestBody->setResourceGroupId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG');
$requestRequestBody->setVirtualNetworkId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET');
$requestRequestBody->setSubnetId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.cloudPcOnPremisesConnection',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->onPremisesConnections()->post($requestRequestBody);


```