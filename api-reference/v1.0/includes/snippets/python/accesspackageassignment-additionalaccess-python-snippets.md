---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AccessPackageAssignmentRequestBuilderGetRequestConfiguration(
request_configuration = AccessPackageAssignmentRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageAssignmentRequestBuilderGetQueryParameters()
query_params['expand'] = ["target"]

)
query_params = AccessPackageAssignmentRequestBuilderGetQueryParameters()
query_params['expand'] = ["target"]

)


result = await client.identityGovernance.entitlementManagement.assignments_by_id('accessPackageAssignment-id').get(request_configuration)


```