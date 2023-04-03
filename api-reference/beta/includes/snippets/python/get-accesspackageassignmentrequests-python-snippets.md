---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration();

queryParameters = AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters();
queryParameters.expand = ["requestor($expand=connectedOrganization)"];
queryParameters.filter = "(requestState eq 'PendingApproval')";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests().get(requestConfiguration);


```