---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.setDisplayName('myGroup')



result = await client.sites._by_id('site-id').termStore.groups.post(request_body)


```