---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => '87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187',
	"displayName" => 'All Users',
	"description" => 'All users can request for access to the directory.',
	"allowedTargetScope" => 'allDirectoryUsers',
	"specificAllowedTargets" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityGovernance()->entitlementManagement()->assignmentPoliciesById('accessPackageAssignmentPolicy-id')->put($requestRequestBody);


```