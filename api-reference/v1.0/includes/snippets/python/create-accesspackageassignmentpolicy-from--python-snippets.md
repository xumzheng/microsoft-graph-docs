---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageAssignmentPolicy();
requestBody.setDisplayName('New Policy');

requestBody.setDescription('policy for assignment');

requestBody.setAllowedTargetScope(AllowedTargetScope('notspecified'));

requestBody.setSpecificAllowedTargets([]);

expiration = ExpirationPattern();
Expiration.setEndDateTime(null);

Expiration.setDuration(null);

expiration.setType(ExpirationPatternType('noexpiration'));


requestBody.setExpiration($expiration);
requestorSettings = AccessPackageAssignmentRequestorSettings();
requestorSettings.setEnableTargetsToSelfAddAccess(false);

requestorSettings.setEnableTargetsToSelfUpdateAccess(false);

requestorSettings.setEnableTargetsToSelfRemoveAccess(false);

requestorSettings.setAllowCustomAssignmentSchedule(true);

requestorSettings.setEnableOnBehalfRequestorsToAddAccess(false);

requestorSettings.setEnableOnBehalfRequestorsToUpdateAccess(false);

requestorSettings.setEnableOnBehalfRequestorsToRemoveAccess(false);

requestorSettings.setOnBehalfRequestors([]);


requestBody.setRequestorSettings($requestorSettings);
requestApprovalSettings = AccessPackageAssignmentApprovalSettings();
requestApprovalSettings.setIsApprovalRequiredForAdd(false);

requestApprovalSettings.setIsApprovalRequiredForUpdate(false);

requestApprovalSettings.setStages([]);


requestBody.setRequestApprovalSettings($requestApprovalSettings);
accessPackage = AccessPackage();
accessPackage.setId('a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b');


requestBody.setAccessPackage($accessPackage);


result = awaitclient.identityGovernance().entitlementManagement().assignmentPolicies().post(requestBody);


```