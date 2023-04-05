---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MembersRequestBuilderGetRequestConfiguration()

query_params = MembersRequestBuilderGetQueryParameters()
query_params.filter = "(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')"

request_config.queryParameters = query_params


result = await client.teamsby_id('team-id')_members.get(request_config)


```