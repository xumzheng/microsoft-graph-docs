---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = GetPresencesByUserIdPostRequestBody();
requestBody.setIds(['fa8bf3dc-eca7-46b7-bad1-db199b62afc3', '66825e03-7ef5-42da-9069-724602c31f6b', ]);



requestResult = graphServiceClient.communications().getPresencesByUserId().post(requestBody);


```