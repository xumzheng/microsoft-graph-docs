---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration();

query_params = AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters;
query_params.expand = ["requestor($expand=connectedOrganization)"];
query_params.filter = "(requestState eq 'PendingApproval')";

request_config.queryParameters = query_params;


result = await client.identityGovernance().entitlementManagement().accessPackageAssignmentRequests().get(request_config);


```