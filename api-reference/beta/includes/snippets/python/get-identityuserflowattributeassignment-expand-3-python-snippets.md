---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = IdentityUserFlowAttributeAssignmentRequestBuilderGetRequestConfiguration();

query_params = IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters();
query_params.expand = ["userAttribute"];

request_config.queryParameters = query_params;


result = await client.identity.b2cUserFlowsById('b2cIdentityUserFlow-id').userAttributeAssignmentsById('identityUserFlowAttributeAssignment-id').get(request_config);


```