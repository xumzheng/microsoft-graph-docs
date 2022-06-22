---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentRequest();


$requestRequestBody->setRequestType(new AccessPackageRequestType('userAdd'));

$assignment = new AccessPackageAssignment();
$requestRequestBody->setAssignment($assignment);


$assignmentAdditionalData = [
	"accessPackageId" => 'd7be3253-b9c6-4fab-adef-30d30de8da2b',
];
$assignment->setAdditionalData($assignmentAdditionalData);

$result =  $graphClient->identityGovernance()->entitlementManagement()->assignmentRequests()->post($requestRequestBody);


```