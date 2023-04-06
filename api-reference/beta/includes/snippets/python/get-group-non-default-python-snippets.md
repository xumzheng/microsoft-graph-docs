---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = GroupRequestBuilderGetRequestConfiguration(
request_configuration = GroupRequestBuilderGetRequestConfiguration(query_params=query_params = GroupRequestBuilderGetQueryParameters()
query_params['select'] = ["allowExternalSenders","autoSubscribeNewMembers","isSubscribedByMail","unseenCount"]

)
query_params = GroupRequestBuilderGetQueryParameters()
query_params['select'] = ["allowExternalSenders","autoSubscribeNewMembers","isSubscribedByMail","unseenCount"]

)


result = await client.groups_by_id('group-id').get(request_configuration)


```