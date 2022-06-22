---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy();


$requestRequestBody->setDisplayName('New Policy');
$requestRequestBody->setDescription('policy for assignment');
$requestRequestBody->setAllowedTargetScope(new AllowedTargetScope('notSpecified'));
$specificAllowedTargetsArray = [];
$requestRequestBody->setSpecificAllowedTargets($specificAllowedTargetsArray);

$expiration = new ExpirationPattern();
$requestRequestBody->setExpiration($expiration);


$expiration->setEndDateTime(null);
$expiration->setDuration(null);
$expiration->setType(new ExpirationPatternType('noExpiration'));


$requestorSettings = new AccessPackageAssignmentRequestorSettings();
$requestRequestBody->setRequestorSettings($requestorSettings);


$requestorSettings->setEnableTargetsToSelfAddAccess(False);
$requestorSettings->setEnableTargetsToSelfUpdateAccess(False);
$requestorSettings->setEnableTargetsToSelfRemoveAccess(False);
$requestorSettings->setAllowCustomAssignmentSchedule(True);
$requestorSettings->setEnableOnBehalfRequestorsToAddAccess(False);
$requestorSettings->setEnableOnBehalfRequestorsToUpdateAccess(False);
$requestorSettings->setEnableOnBehalfRequestorsToRemoveAccess(False);
$onBehalfRequestorsArray = [];
$requestorSettings->setOnBehalfRequestors($onBehalfRequestorsArray);


$requestApprovalSettings = new AccessPackageAssignmentApprovalSettings();
$requestRequestBody->setRequestApprovalSettings($requestApprovalSettings);


$requestApprovalSettings->setIsApprovalRequiredForAdd(False);
$requestApprovalSettings->setIsApprovalRequiredForUpdate(False);
$stagesArray = [];
$requestApprovalSettings->setStages($stagesArray);


$accessPackage = new AccessPackage();
$requestRequestBody->setAccessPackage($accessPackage);


$accessPackage->setId('a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b');

$result =  $graphClient->identityGovernance()->entitlementManagement()->assignmentPolicies()->post($requestRequestBody);


```