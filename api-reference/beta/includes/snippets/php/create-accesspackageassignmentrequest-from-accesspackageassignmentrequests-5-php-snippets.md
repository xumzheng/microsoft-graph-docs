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



$target = new AccessPackageSubject();
$accessPackageAssignment->setTarget($target);


$target->setEmail('user@contoso.com');

$accessPackageAssignment->setAssignmentPolicyId('2264bf65-76ba-417b-a27d-54d291f0cbc8');
$accessPackageAssignment->setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentRequests()->post($requestRequestBody);


```