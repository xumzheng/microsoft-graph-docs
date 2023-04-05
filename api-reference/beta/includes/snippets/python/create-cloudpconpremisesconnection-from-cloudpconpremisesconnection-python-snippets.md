---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcOnPremisesConnection()
request_body.setDisplayName('test-canary-02')

request_body.setType(CloudPcOnPremisesConnectionType('hybridazureadjoin'))

request_body.setSubscriptionId('0ac520ee-14c0-480f-b6c9-0a90c585ffff')

request_body.setAdDomainName('contoso001.com')

request_body.setAdDomainUsername('dcadmin')

request_body.setOrganizationalUnit('OU=Domain Controllers, DC=contoso001, DC=com')

request_body.setResourceGroupId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG')

request_body.setVirtualNetworkId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET')

request_body.setSubnetId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet')



result = await client.deviceManagement_virtualEndpoint_onPremisesConnections.post(request_body)


```