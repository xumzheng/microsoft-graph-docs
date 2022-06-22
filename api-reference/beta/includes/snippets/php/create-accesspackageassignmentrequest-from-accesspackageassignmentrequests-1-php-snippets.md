---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentRequest();


$requestRequestBody->setRequestType('AdminAdd');

$accessPackageAssignment = new AccessPackageAssignment();
$requestRequestBody->setAccessPackageAssignment($accessPackageAssignment);


$accessPackageAssignment->setTargetId('46184453-e63b-4f20-86c2-c557ed5d5df9');
$accessPackageAssignment->setAssignmentPolicyId('2264bf65-76ba-417b-a27d-54d291f0cbc8');
$accessPackageAssignment->setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentRequests()->post($requestRequestBody);


```