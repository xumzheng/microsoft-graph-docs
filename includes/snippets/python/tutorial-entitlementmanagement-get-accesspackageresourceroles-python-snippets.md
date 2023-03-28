---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AccessPackageResourceRolesRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageResourceRolesRequestBuilderGetQueryParameters();
$queryParameters.filter = "(originSystem eq 'AadGroup' and accessPackageResource/id eq '4a1e21c5-8a76-4578-acb1-641160e076e8' and displayName eq 'Member')";
$queryParameters.expand = ["accessPackageResource"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').accessPackageResourceRoles().get($requestConfiguration);


```