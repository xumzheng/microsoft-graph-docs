---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ConnectedOrganization();
request_body.setDisplayName('Connected organization name');

request_body.setDescription('Connected organization description');

identitySourcesIdentitySource1 = IdentitySource();
identitySourcesIdentitySource1.set@odatatype('#microsoft.graph.domainIdentitySource');

additionalData = [
'domainName' => 'example.com', 
'displayName' => 'example.com', 
];
identitySourcesIdentitySource1.setAdditionalData(additionalData);



identitySourcesArray []= identitySourcesIdentitySource1;
request_body.setIdentitySources(identitySourcesArray);


request_body.setState(ConnectedOrganizationState('proposed'));



result = await client.identityGovernance().entitlementManagement().connectedOrganizations().post(request_body);


```