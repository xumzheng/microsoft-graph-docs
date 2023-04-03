---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = UserAttributeAssignmentsRequestBuilderGetRequestConfiguration();

query_params = UserAttributeAssignmentsRequestBuilderGetQueryParameters();
query_params.expand = ["userAttribute"];

request_config.queryParameters = query_params;


result = awaitclient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').userAttributeAssignments().get(request_config);


```