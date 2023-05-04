---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Add_large_gallery_view_post_request_body()
request_body.client_context = '785f4929-92ca-497b-863f-c778c77c9758'




result = await client.communications.calls.by_call_id('call-id').add_large_gallery_view.post(request_body = request_body)


```