---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration(
request_configuration = AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters()
query_params['expand'] = ["requestor($expand=connectedOrganization)"]
query_params['filter'] = "(requestState eq 'PendingApproval')"

)
query_params = AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters()
query_params['expand'] = ["requestor($expand=connectedOrganization)"]
query_params['filter'] = "(requestState eq 'PendingApproval')"

)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.get(request_configuration)


```