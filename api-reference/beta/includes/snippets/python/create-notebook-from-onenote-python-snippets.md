---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Notebook();
requestBody.setDisplayName('My Private notebook');



result = await client.me().onenote().notebooks().post(requestBody);


```