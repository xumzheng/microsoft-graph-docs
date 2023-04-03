---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AccessPackageResourcesRequestBuilderGetRequestConfiguration();

queryParameters = AccessPackageResourcesRequestBuilderGetQueryParameters();
queryParameters.filter = "resourceType eq 'Application'";
queryParameters.expand = ["accessPackageResourceScopes"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').accessPackageResources().get(requestConfiguration);


```