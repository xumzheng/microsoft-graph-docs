---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AccessPackageCatalogsRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageCatalogsRequestBuilderGetQueryParameters();
$queryParameters.filter = "(displayName eq 'General')";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().accessPackageCatalogs().get($requestConfiguration);


```