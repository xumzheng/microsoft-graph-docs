---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MailFoldersRequestBuilderGetRequestConfiguration(
request_config = MailFoldersRequestBuilderGetRequestConfiguration(query_params=query_params = MailFoldersRequestBuilderGetQueryParameters()
query_params.includehiddenfolders = true

)
query_params = MailFoldersRequestBuilderGetQueryParameters()
query_params.includehiddenfolders = true

)


result = await client.me.mailFolders.get(request_config, headers=request_config)


```