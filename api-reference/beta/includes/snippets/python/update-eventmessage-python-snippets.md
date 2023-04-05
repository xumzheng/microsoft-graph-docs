---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.setIsRead(true)



result = await client.me.messages._by_id('message-id').patch(request_body)


```