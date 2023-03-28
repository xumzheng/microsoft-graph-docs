---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AttachmentRequestBuilderGetRequestConfiguration();

$queryParameters = new AttachmentRequestBuilderGetQueryParameters();
$queryParameters.expand = ["microsoft.graph.itemattachment/item"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().messagesById('message-id').attachmentsById('attachment-id').get($requestConfiguration);


```