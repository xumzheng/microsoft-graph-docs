---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PinnedMessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new PinnedMessagesRequestBuilderGetQueryParameters();
$queryParameters->expand = ["message"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->chatsById('chat-id')->pinnedMessages()->get($requestConfiguration);


```