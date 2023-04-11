---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcOnPremisesConnection()
request_body.@odatatype = '#microsoft.graph.cloudPcOnPremisesConnection'

request_body.displayName = 'Display Name value'

request_body.subscriptionId = '0ac520ee-14c0-480f-b6c9-0a90c585ffff'

request_body.subscriptionName = 'Subscription Name value'

request_body.adDomainName = 'Active Directory Domain Name value'

request_body.adDomainUsername = 'Active Directory Domain User Name value'

request_body.organizationalUnit = 'Organization Unit value'

request_body.resourceGroupId = '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG'

request_body.virtualNetworkId = '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet'

request_body.subnetId = '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default'




result = await client.deviceManagement.virtualEndpoint.onPremisesConnections_by_id('cloudPcOnPremisesConnection-id').patch(request_body = request_body)


```