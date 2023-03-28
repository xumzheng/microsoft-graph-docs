---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConnectedOrganization();
$requestBody->setDisplayName('Connected organization name');

$requestBody->setDescription('Connected organization description');

$identitySourcesIdentitySource1 = new IdentitySource();
$identitySourcesIdentitySource1->set@odatatype('#microsoft.graph.domainIdentitySource');

$additionalData = [
'domainName' => 'example.com', 
'displayName' => 'example.com', 
];
$identitySourcesIdentitySource1->setAdditionalData($additionalData);



$identitySourcesArray []= $identitySourcesIdentitySource1;
$requestBody->setIdentitySources($identitySourcesArray);


$requestBody->setState(new ConnectedOrganizationState('proposed'));



$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->connectedOrganizations()->post($requestBody);


```