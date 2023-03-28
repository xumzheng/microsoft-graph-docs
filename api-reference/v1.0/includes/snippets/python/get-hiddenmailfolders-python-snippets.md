---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new MailFoldersRequestBuilderGetRequestConfiguration();

$queryParameters = new MailFoldersRequestBuilderGetQueryParameters();
$queryParameters->includehiddenfolders = true;

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->me()->mailFolders()->get($requestConfiguration);


```