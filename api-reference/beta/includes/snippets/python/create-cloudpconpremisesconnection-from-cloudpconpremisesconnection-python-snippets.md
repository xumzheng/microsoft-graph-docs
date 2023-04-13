---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcOnPremisesConnection()
request_body.displayName = 'test-canary-02'

request_body.Type(CloudPcOnPremisesConnectionType('hybridazureadjoin'))

request_body.subscriptionId = '0ac520ee-14c0-480f-b6c9-0a90c585ffff'

request_body.adDomainName = 'contoso001.com'

request_body.adDomainUsername = 'dcadmin'

request_body.organizationalUnit = 'OU=Domain Controllers, DC=contoso001, DC=com'

request_body.resourceGroupId = '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG'

request_body.virtualNetworkId = '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET'

request_body.subnetId = '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet'




result = await client.deviceManagement.virtualEndpoint.onPremisesConnections.post(request_body = request_body)


```