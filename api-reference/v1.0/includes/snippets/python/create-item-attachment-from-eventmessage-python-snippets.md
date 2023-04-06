---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.set@odatatype('#Microsoft.OutlookServices.ItemAttachment')

request_body.setName('name-value')

additionalData = [
'item' => request_body = Item()
		request_body.set@odatatype('microsoft.graph.message')


request_body.setItem($item)

];
request_body.setAdditionalData(additionalData)




result = await client.me.events_by_id('event-id').attachments.post(request_body, headers=)


```