---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OutlookTaskGroup();
requestBody.setName('Leisure tasks');



result = await client.me().outlook().taskGroups().post(requestBody);


```