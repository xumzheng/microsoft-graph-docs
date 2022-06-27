---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => 'b2eba9a1-b357-42ee-83a8-336522ed6cbf',
	"accessPackageId" => '4c02f928-7752-49aa-8fc8-e286d973a965',
	"displayName" => 'All Users',
	"description" => 'All users can request for access to the directory.',
	"canExtend" => False,
	"durationInDays" => 365,
	"expirationDateTime" => null,
	"questions" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentPoliciesById('accessPackageAssignmentPolicy-id')->put($requestRequestBody);


```