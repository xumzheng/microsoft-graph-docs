---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PinnedMessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new PinnedMessagesRequestBuilderGetQueryParameters();
$queryParameters->expand = 'message';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->chatsById('chat-id')->pinnedMessages()->get($requestConfiguration);


```