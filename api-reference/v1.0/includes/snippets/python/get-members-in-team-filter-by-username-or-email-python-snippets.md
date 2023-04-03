---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = MembersRequestBuilderGetRequestConfiguration();

query_params = MembersRequestBuilderGetQueryParameters();
query_params.filter = "(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')";

request_config.queryParameters = query_params;


result = awaitclient.teamsById('team-id').members().get(request_config);


```