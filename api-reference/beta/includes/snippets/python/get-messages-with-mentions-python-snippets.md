---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters.filter = "MentionsPreview/IsMentioned eq true";
$queryParameters.select = ["Subject","Sender","ReceivedDateTime","MentionsPreview"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().messages().get($requestConfiguration);


```