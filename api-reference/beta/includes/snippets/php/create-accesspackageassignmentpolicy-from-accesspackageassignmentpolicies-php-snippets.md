---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy();


$requestRequestBody->setAccessPackageId('56ff43fd-6b05-48df-9634-956a777fce6d');
$requestRequestBody->setDisplayName('direct');
$requestRequestBody->setDescription('direct assignments by administrator');
$requestRequestBody->setAccessReviewSettings(null);

$requestorSettings = new RequestorSettings();
$requestRequestBody->setRequestorSettings($requestorSettings);


$requestorSettings->setScopeType('NoSubjects');
$requestorSettings->setAcceptRequests(True);
$allowedRequestorsArray = [];
$requestorSettings->setAllowedRequestors($allowedRequestorsArray);


$requestApprovalSettings = new ApprovalSettings();
$requestRequestBody->setRequestApprovalSettings($requestApprovalSettings);


$requestApprovalSettings->setIsApprovalRequired(False);
$requestApprovalSettings->setIsApprovalRequiredForExtension(False);
$requestApprovalSettings->setIsRequestorJustificationRequired(False);
$requestApprovalSettings->setApprovalMode('NoApproval');
$approvalStagesArray = [];
$requestApprovalSettings->setApprovalStages($approvalStagesArray);

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentPolicies()->post($requestRequestBody);


```