---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.@odatatype = '#Microsoft.OutlookServices.ItemAttachment'

request_body.name = 'name-value'

additionalData = [
'item' => request_body = Item()
		request_body.@odatatype = 'microsoft.graph.message'


request_body.item = item

];
request_body.additionaldata(additionalData)





result = await client.me.events_by_id('event-id').attachments.post(request_body = request_body)


```