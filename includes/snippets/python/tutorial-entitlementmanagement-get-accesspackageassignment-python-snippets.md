---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AccessPackageAssignmentsRequestBuilder.AccessPackageAssignmentsRequestBuilderGetQueryParameters(
				filter = "accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'",
				expand = ["target","accessPackageAssignmentResourceRoles"],
)

request_configuration = AccessPackageAssignmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignments.get(request_configuration = request_configuration)


```