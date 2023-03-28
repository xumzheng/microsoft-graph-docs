---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ChildFoldersRequestBuilderGetRequestConfiguration();

$queryParameters = new ChildFoldersRequestBuilderGetQueryParameters();
$queryParameters->includehiddenfolders = true;

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->me()->mailFoldersById('mailFolder-id')->childFolders()->get($requestConfiguration);


```