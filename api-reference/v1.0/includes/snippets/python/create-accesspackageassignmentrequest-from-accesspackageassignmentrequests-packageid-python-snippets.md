---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessPackageAssignmentRequest();
$requestBody->setRequestType(new AccessPackageRequestType('useradd'));

$assignment = new AccessPackageAssignment();
$additionalData = [
'accessPackageId' => 'd7be3253-b9c6-4fab-adef-30d30de8da2b', 
];
$assignment->setAdditionalData($additionalData);



$requestBody->setAssignment($assignment);


$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->assignmentRequests()->post($requestBody);


```