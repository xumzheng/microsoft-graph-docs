---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.set@odatatype('#microsoft.graph.itemAttachment')

request_body.setName('Holiday event')

additionalData = [
'item' => request_body = Item()
		request_body.set@odatatype('microsoft.graph.event')

		request_body.setSubject('Discuss gifts for children')

body = Body()
		body.setContentType('HTML')

		body.setContent('Let\'s look for funding!')


request_body.setBody($body)
start = Start()
		start.setDateTime('2016-12-02T18:00:00')

		start.setTimeZone('Pacific Standard Time')


request_body.setStart($start)
end = End()
		end.setDateTime('2016-12-02T19:00:00')

		end.setTimeZone('Pacific Standard Time')


request_body.setEnd($end)

request_body.setItem($item)

];
request_body.setAdditionalData(additionalData)




result = await client.me.messages_by_id('message-id').attachments.post(request_body, headers=)


```