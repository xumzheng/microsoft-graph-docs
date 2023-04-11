---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemPatent()
request_body.number = 'USPTO-3954432633'

request_body.webUrl = 'https://patents.gov/3954432633'



request_configuration = ItemPatentRequestBuilderPatchRequestConfiguration(
)


result = await client.users_by_id('user-id').profile.patents_by_id('itemPatent-id').patch(request_body = request_body)


```