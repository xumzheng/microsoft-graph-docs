---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters();
$queryParameters->expand = 'customExtensionHandlers($expand=customExtension)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentPoliciesById('accessPackageAssignmentPolicy-id')->get($requestConfiguration);


```