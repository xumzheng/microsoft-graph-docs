---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TodoTaskList();
requestBody.setDisplayName('Travel items');



result = awaitclient.me().todo().lists().post(requestBody);


```