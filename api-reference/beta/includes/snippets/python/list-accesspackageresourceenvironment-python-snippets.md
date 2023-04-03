---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AccessPackageResourceEnvironmentsRequestBuilderGetRequestConfiguration();

queryParameters = AccessPackageResourceEnvironmentsRequestBuilderGetQueryParameters();
queryParameters.filter = "originSystem eq 'SharePointOnline'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageResourceEnvironments().get(requestConfiguration);


```