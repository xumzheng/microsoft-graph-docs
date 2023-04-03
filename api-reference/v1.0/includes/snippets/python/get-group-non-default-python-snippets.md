---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = GroupRequestBuilderGetRequestConfiguration();

query_params = GroupRequestBuilderGetQueryParameters();
query_params.select = ["allowExternalSenders","autoSubscribeNewMembers","isSubscribedByMail","unseenCount"];

request_config.queryParameters = query_params;


result = awaitclient.groupsById('group-id').get(request_config);


```