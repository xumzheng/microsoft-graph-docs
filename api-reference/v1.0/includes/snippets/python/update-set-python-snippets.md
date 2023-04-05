---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Set()
request_body.setDescription('mySet')



result = await client.sites._by_id('site-id').termStore.sets._by_id('set-id').patch(request_body)


```