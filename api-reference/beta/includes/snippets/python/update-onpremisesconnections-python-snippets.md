---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcOnPremisesConnection()
request_body.set@odatatype('#microsoft.graph.cloudPcOnPremisesConnection')

request_body.setDisplayName('Display Name value')

request_body.setSubscriptionId('0ac520ee-14c0-480f-b6c9-0a90c585ffff')

request_body.setSubscriptionName('Subscription Name value')

request_body.setAdDomainName('Active Directory Domain Name value')

request_body.setAdDomainUsername('Active Directory Domain User Name value')

request_body.setOrganizationalUnit('Organization Unit value')

request_body.setResourceGroupId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG')

request_body.setVirtualNetworkId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet')

request_body.setSubnetId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default')



result = await client.deviceManagement.virtualEndpoint.onPremisesConnectionsby_id('cloudPcOnPremisesConnection-id').patch(request_body)


```