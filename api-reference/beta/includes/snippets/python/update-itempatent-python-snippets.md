---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemPatent()
request_body.setNumber('USPTO-3954432633')

request_body.setWebUrl('https://patents.gov/3954432633')



result = await client.usersby_id('user-id').profile.patentsby_id('itemPatent-id').patch(request_body)


```