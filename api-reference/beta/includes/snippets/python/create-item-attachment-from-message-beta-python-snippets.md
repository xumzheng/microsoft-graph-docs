---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.@odatatype = '#microsoft.graph.itemAttachment'

request_body.name = 'Holiday event'

additionalData = [
'item' => request_body = Item()
		request_body.@odatatype = 'microsoft.graph.event'

		request_body.subject = 'Discuss gifts for children'

body = Body()
		body.contentType = 'HTML'

		body.content = 'Let\'s look for funding!'


request_body.body = body
start = Start()
		start.dateTime = '2016-12-02T18:00:00'

		start.timeZone = 'Pacific Standard Time'


request_body.start = start
end = End()
		end.dateTime = '2016-12-02T19:00:00'

		end.timeZone = 'Pacific Standard Time'


request_body.end = end

request_body.item = item

];
request_body.additionaldata(additionalData)





result = await client.me.messages_by_id('message-id').attachments.post(request_body = request_body)


```