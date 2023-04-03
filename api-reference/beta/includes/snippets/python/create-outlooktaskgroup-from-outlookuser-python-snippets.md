---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OutlookTaskGroup();
requestBody.setName('Leisure tasks');



requestResult = graphServiceClient.me().outlook().taskGroups().post(requestBody);


```