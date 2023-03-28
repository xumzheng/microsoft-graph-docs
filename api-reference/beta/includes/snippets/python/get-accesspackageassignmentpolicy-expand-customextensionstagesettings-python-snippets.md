---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters();
$queryParameters.expand = ["customExtensionStageSettings($expand=customExtension)"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().accessPackageAssignmentPoliciesById('accessPackageAssignmentPolicy-id').get($requestConfiguration);


```