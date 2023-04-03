---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/v1.0/groups/{id}');



graphServiceClient.directory().administrativeUnitsById('administrativeUnit-id').members().ref().post(requestBody);


```