---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AccessPackageRequestBuilderGetRequestConfiguration();

queryParameters = AccessPackageRequestBuilderGetQueryParameters();
queryParameters.expand = ["accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').get(requestConfiguration);


```