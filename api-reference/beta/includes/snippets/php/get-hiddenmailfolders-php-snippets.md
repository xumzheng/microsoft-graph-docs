---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MailFoldersRequestBuilderGetRequestConfiguration();

$queryParameters = new MailFoldersRequestBuilderGetQueryParameters();
$queryParameters->includeHiddenFolders = true;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->mailFolders()->get($requestConfiguration);


```