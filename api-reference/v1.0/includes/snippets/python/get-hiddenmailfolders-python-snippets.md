---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MailFoldersRequestBuilderGetRequestConfiguration();

queryParameters = MailFoldersRequestBuilderGetQueryParameters();
queryParameters.includehiddenfolders = true;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().mailFolders().get(requestConfiguration);


```