---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration(
request_config = AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["requestor($expand=connectedOrganization)"]
params['filter'] = "(requestState eq 'PendingApproval')"
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.get(request_config, headers=request_config)


```