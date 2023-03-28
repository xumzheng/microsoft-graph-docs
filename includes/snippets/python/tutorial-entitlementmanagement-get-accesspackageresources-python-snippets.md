---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AccessPackageResourcesRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageResourcesRequestBuilderGetQueryParameters();
$queryParameters->filter = "(displayName eq 'Marketing resources')";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->accessPackageCatalogsById('accessPackageCatalog-id')->accessPackageResources()->get($requestConfiguration);


```