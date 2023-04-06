---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ChildFoldersRequestBuilderGetRequestConfiguration(
request_configuration = ChildFoldersRequestBuilderGetRequestConfiguration(query_params=query_params = ChildFoldersRequestBuilderGetQueryParameters()
query_params['includehiddenfolders'] = true

)
query_params = ChildFoldersRequestBuilderGetQueryParameters()
query_params['includehiddenfolders'] = true

)


result = await client.me.mailFolders_by_id('mailFolder-id').childFolders.get(request_configuration)


```