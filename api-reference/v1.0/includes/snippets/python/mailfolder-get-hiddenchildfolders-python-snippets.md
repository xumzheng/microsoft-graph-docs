---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ChildFoldersRequestBuilderGetRequestConfiguration(
request_config = ChildFoldersRequestBuilderGetRequestConfiguration(query_params=params['includehiddenfolders'] = true
)


result = await client.me.mailFolders_by_id('mailFolder-id').childFolders.get(request_config, headers=request_config)


```