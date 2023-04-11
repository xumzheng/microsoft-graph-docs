---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = AttachmentRequestBuilderGetRequestConfiguration(
)


result = await client.me.events_by_id('event-id').attachments_by_id('attachment-id').get()


```