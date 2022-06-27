---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => '4540a08f-8ab5-43f6-a923-015275799197',
	"displayName" => 'policy with custom access package workflow extension',
	"description" => 'Run specified custom access package workflow extension at different stages.',
	"accessPackageId" => 'ba5807c7-2aa9-4c8a-907e-4a17ee587500',
	"requestApprovalSettings" => null,
	"accessReviewSettings" => null,
	"customExtensionHandlers" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentPoliciesById('accessPackageAssignmentPolicy-id')->put($requestRequestBody);


```