---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageAssignmentsRequestBuilderGetRequestConfiguration(
request_config = AccessPackageAssignmentsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'"
params['expand'] = ["target","accessPackageAssignmentResourceRoles"]
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignments.get(request_config, headers=request_config)


```