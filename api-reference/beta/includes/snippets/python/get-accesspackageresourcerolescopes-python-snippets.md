---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AccessPackageRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageRequestBuilderGetQueryParameters();
$queryParameters.expand = ["accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').get($requestConfiguration);


```