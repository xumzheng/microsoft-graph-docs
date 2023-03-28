---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ChatsRequestBuilderGetRequestConfiguration();

$queryParameters = new ChatsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["lastMessagePreview"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->chats()->get($requestConfiguration);


```