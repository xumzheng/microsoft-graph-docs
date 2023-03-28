---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConnectedOrganization();
$requestBody.setDisplayName('Connected organization new name');

$requestBody.setDescription('Connected organization new description');

$requestBody.setState(new ConnectedOrganizationState('configured'));



$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().connectedOrganizationsById('connectedOrganization-id').patch($requestBody);


```