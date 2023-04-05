---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AttachmentRequestBuilderGetRequestConfiguration()

query_params = AttachmentRequestBuilderGetQueryParameters()
query_params.expand = ["microsoft.graph.itemattachment/item"]

request_config.queryParameters = query_params


result = await client.me_messagesby_id('message-id')_attachmentsby_id('attachment-id').get(request_config)


```