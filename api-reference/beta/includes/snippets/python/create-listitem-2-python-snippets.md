---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = FieldValueSet();
additionalData = [
'Color' => 'Fuchsia', 
'Quantity' => 934,
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.sitesById('site-id').listsById('list-id').itemsById('listItem-id').fields().patch(requestBody);


```