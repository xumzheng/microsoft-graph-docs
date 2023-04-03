---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration();

query_params = PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters();
query_params.filter = "isElevated eq true and expirationDateTime ne null or isElevated eq false";

request_config.queryParameters = query_params;


result = await client.privilegedRoleAssignments().get(request_config);


```