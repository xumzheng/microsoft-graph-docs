---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters->top = 2;
$queryParameters->orderBy = 'createdDateTime%20desc';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->chatsById('chat-id')->messages()->get($requestConfiguration);


```