---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ChildFoldersRequestBuilderGetRequestConfiguration();

$queryParameters = new ChildFoldersRequestBuilderGetQueryParameters();
$queryParameters->includeHiddenFolders = true;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->mailFoldersById('mailFolder-id')->childFolders()->get($requestConfiguration);


```