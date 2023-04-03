---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = FieldValueSet();
additionalData = [
'Color' => 'Fuchsia', 
'Quantity' => 934,
];
requestBody.setAdditionalData(additionalData);




result = await client.sitesById('site-id').listsById('list-id').itemsById('listItem-id').fields().patch(requestBody);


```