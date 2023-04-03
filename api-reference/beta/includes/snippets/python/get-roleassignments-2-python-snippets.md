---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration();

query_params = RoleAssignmentsRequestBuilderGetQueryParameters();
query_params.filter = " principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'";

request_config.queryParameters = query_params;


result = await client.roleManagement().directory().roleAssignments().get(request_config);


```