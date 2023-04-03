---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OutlookTaskGroup();
requestBody.setName('Personal Tasks');



result = await client.me().outlook().taskGroupsById('outlookTaskGroup-id').patch(requestBody);


```