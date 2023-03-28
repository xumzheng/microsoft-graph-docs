---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new GetAllMessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new GetAllMessagesRequestBuilderGetQueryParameters();
$queryParameters->top = 2;

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->usersById('user-id')->chats()->getAllMessages()->get($requestConfiguration);


```