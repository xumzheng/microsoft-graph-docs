---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetUserOwnedObjectsPostRequestBody()
request_body.setUserId('55ac777c-109e-4022-b58c-470c8fcb6892')

request_body.setType('Group')


request_config = GetUserOwnedObjectsRequestBuilderPostRequestConfiguration(
request_config = GetUserOwnedObjectsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.directory.deletedItems.getUserOwnedObjects.post(request_body, headers=)


```