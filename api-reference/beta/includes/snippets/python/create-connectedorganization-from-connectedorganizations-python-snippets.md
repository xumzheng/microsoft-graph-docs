---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConnectedOrganization()
request_body.displayName = 'Connected organization name'

request_body.description = 'Connected organization description'

identitySourcesIdentitySource1 = IdentitySource()
identitySourcesIdentitySource1.@odatatype = '#microsoft.graph.domainIdentitySource'

additionalData = [
'domainName' => 'example.com', 
'displayName' => 'example.com', 
];
identitySourcesIdentitySource1.additionaldata(additionalData)



identitySourcesArray []= identitySourcesIdentitySource1;
request_body.identitysources(identitySourcesArray)


request_body.State(ConnectedOrganizationState('proposed'))




result = await client.identityGovernance.entitlementManagement.connectedOrganizations.post(request_body = request_body)


```