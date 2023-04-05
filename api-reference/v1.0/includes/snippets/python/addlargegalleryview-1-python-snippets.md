---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddLargeGalleryViewPostRequestBody()
request_body.setClientContext('785f4929-92ca-497b-863f-c778c77c9758')



result = await client.communications.calls_by_id('call-id').addLargeGalleryView.post(request_body)


```