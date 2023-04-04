---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration();

query_params = TransitiveRoleAssignmentsRequestBuilderGetQueryParameters();
query_params.count = true;
query_params.filter = "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and directoryScopeId eq '/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2'";

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.roleManagement.directory.transitiveRoleAssignments.get(request_config);


```