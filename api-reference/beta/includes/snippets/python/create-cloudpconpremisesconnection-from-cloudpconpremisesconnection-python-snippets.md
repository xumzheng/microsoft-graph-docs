---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CloudPcOnPremisesConnection();
$requestBody->setDisplayName('test-canary-02');

$requestBody->setType(new CloudPcOnPremisesConnectionType('hybridazureadjoin'));

$requestBody->setSubscriptionId('0ac520ee-14c0-480f-b6c9-0a90c585ffff');

$requestBody->setAdDomainName('contoso001.com');

$requestBody->setAdDomainUsername('dcadmin');

$requestBody->setOrganizationalUnit('OU=Domain Controllers, DC=contoso001, DC=com');

$requestBody->setResourceGroupId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG');

$requestBody->setVirtualNetworkId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET');

$requestBody->setSubnetId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet');



$requestResult = $graphServiceClient->deviceManagement()->virtualEndpoint()->onPremisesConnections()->post($requestBody);


```