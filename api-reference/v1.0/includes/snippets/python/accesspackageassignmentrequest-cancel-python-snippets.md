---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = CancelRequestBuilderPostRequestConfiguration(
)


await client.identityGovernance.entitlementManagement.assignmentRequests_by_id('accessPackageAssignmentRequest-id').cancel.post()


```