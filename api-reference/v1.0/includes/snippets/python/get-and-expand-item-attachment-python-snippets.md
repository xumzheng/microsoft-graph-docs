---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = AttachmentRequestBuilderGetRequestConfiguration();

query_params = AttachmentRequestBuilderGetQueryParameters();
query_params.expand = ["microsoft.graph.itemattachment/item"];

request_config.queryParameters = query_params;


result = awaitclient.me().messagesById('message-id').attachmentsById('attachment-id').get(request_config);


```