---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemPublication()
request_body.setPublisher('International Association of Branding Management Publishing')

request_body.setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg')



result = await client.users._by_id('user-id').profile.publications._by_id('itemPublication-id').patch(request_body)


```