---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OutlookTaskGroup();
requestBody.setName('Personal Tasks');



result = awaitclient.me().outlook().taskGroupsById('outlookTaskGroup-id').patch(requestBody);


```