---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/v1.0/groups/{groupId}');



graphServiceClient.print().sharesById('printerShare-id').allowedGroups().ref().post(requestBody);


```