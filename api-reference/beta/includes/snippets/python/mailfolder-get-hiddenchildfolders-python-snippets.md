---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ChildFoldersRequestBuilder.ChildFoldersRequestBuilderGetQueryParameters(
				includehiddenfolders = true,
)

request_configuration = ChildFoldersRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.me.mailFolders_by_id('mailFolder-id').childFolders.get(request_configuration = request_configuration)


```