---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters.top = 2;

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.chatsById('chat-id').messages().get($requestConfiguration);


```