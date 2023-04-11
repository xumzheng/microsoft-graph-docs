---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = MailFoldersRequestBuilder.MailFoldersRequestBuilderGetQueryParameters(
				includehiddenfolders = true,
)

request_configuration = MailFoldersRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.me.mailFolders.get(request_configuration = request_configuration)


```