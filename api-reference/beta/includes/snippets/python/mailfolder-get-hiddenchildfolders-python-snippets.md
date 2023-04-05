---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ChildFoldersRequestBuilderGetRequestConfiguration()

query_params = ChildFoldersRequestBuilderGetQueryParameters()
query_params.includehiddenfolders = true

request_config.queryParameters = query_params


result = await client.me.mailFoldersby_id('mailFolder-id').childFolders.get(request_config)


```