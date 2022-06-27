---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentRequest();


$requestRequestBody->setRequestType('AdminRemove');

$accessPackageAssignment = new AccessPackageAssignment();
$requestRequestBody->setAccessPackageAssignment($accessPackageAssignment);


$accessPackageAssignment->setId('a6bb6942-3ae1-4259-9908-0133aaee9377');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentRequests()->post($requestRequestBody);


```