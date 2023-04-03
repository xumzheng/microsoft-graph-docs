---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ItemPhone();
requestBody.setType(PhoneType('other'));



result = awaitclient.usersById('user-id').profile().phonesById('itemPhone-id').patch(requestBody);


```