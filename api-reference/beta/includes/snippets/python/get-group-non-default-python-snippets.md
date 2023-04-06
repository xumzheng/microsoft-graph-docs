---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration(
request_config = GroupRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["allowExternalSenders","autoSubscribeNewMembers","isSubscribedByMail","unseenCount"]
)


result = await client.groups_by_id('group-id').get(request_config, headers=request_config)


```