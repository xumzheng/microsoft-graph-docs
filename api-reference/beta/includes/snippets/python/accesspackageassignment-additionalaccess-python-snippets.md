---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageAssignmentRequestBuilderGetRequestConfiguration()

query_params = AccessPackageAssignmentRequestBuilderGetQueryParameters()
query_params.expand = ["target"]

request_config.queryParameters = query_params


result = await client.identityGovernance_entitlementManagement_accessPackageAssignmentsby_id('accessPackageAssignment-id').get(request_config)


```