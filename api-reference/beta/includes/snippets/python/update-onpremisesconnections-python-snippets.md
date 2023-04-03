---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CloudPcOnPremisesConnection();
requestBody.set@odatatype('#microsoft.graph.cloudPcOnPremisesConnection');

requestBody.setDisplayName('Display Name value');

requestBody.setSubscriptionId('0ac520ee-14c0-480f-b6c9-0a90c585ffff');

requestBody.setSubscriptionName('Subscription Name value');

requestBody.setAdDomainName('Active Directory Domain Name value');

requestBody.setAdDomainUsername('Active Directory Domain User Name value');

requestBody.setOrganizationalUnit('Organization Unit value');

requestBody.setResourceGroupId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG');

requestBody.setVirtualNetworkId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet');

requestBody.setSubnetId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default');



result = await client.deviceManagement().virtualEndpoint().onPremisesConnectionsById('cloudPcOnPremisesConnection-id').patch(requestBody);


```