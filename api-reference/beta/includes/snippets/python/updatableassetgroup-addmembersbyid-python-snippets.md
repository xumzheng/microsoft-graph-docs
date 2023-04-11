---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddMembersByIdPostRequestBody()
request_body.Ids(['String', 'String', 'String', ])

request_body.memberEntityType = '#microsoft.graph.windowsUpdates.azureADDevice'



request_configuration = AddMembersByIdRequestBuilderPostRequestConfiguration(
)


await client.admin.windows.updates.updatableAssets_by_id('updatableAsset-id').windowsUpdatesaddMembersById.post(request_body = request_body)


```