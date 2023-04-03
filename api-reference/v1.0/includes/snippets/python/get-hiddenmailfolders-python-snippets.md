---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = MailFoldersRequestBuilderGetRequestConfiguration();

query_params = MailFoldersRequestBuilderGetQueryParameters();
query_params.includehiddenfolders = true;

request_config.queryParameters = query_params;


result = awaitclient.me().mailFolders().get(request_config);


```