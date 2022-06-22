---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ChatRequestBuilderGetRequestConfiguration();

$queryParameters = new ChatRequestBuilderGetQueryParameters();
$queryParameters->expand = 'members';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->chatsById('chat-id')->get($requestConfiguration);


```