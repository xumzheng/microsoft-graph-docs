---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Notebook();
requestBody.setDisplayName('My Private notebook');



result = awaitclient.me().onenote().notebooks().post(requestBody);


```