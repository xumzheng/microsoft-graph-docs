---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OutlookTaskGroup();
requestBody.setName('Leisure tasks');



result = awaitclient.me().outlook().taskGroups().post(requestBody);


```