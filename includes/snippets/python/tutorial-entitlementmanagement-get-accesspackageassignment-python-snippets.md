---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AccessPackageAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->filter = "accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'";
$queryParameters->expand = ["target","accessPackageAssignmentResourceRoles"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->accessPackageAssignments()->get($requestConfiguration);


```