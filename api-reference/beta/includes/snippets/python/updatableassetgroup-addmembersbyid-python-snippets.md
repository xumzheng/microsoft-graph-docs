---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddMembersByIdPostRequestBody()
request_body.setIds(['String', 'String', 'String', ])

request_body.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice')


request_config = AddMembersByIdRequestBuilderPostRequestConfiguration(
request_config = AddMembersByIdRequestBuilderPostRequestConfiguration(query_params=)


await client.admin.windows.updates.updatableAssets_by_id('updatableAsset-id').windowsUpdatesaddMembersById.post(request_body, headers=)


```