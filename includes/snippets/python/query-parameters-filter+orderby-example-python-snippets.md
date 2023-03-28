---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters->filter = "Subject eq 'welcome' and importance eq 'normal'";
$queryParameters->orderby = ["subject","importance","receivedDateTime desc"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->me()->messages()->get($requestConfiguration);


```