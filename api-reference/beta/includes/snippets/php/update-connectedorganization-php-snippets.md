---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConnectedOrganization();


$requestRequestBody->setDisplayName('Connected organization new name');
$requestRequestBody->setDescription('Connected organization new description');
$requestRequestBody->setState(new ConnectedOrganizationState('configured'));
$result =  $graphClient->identityGovernance()->entitlementManagement()->connectedOrganizationsById('connectedOrganization-id')->patch($requestRequestBody);


```