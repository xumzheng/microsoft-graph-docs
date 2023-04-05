---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FieldValueSet()
additionalData = [
'Color' => 'Fuchsia', 
'Quantity' => 934,
];
request_body.setAdditionalData(additionalData)




result = await client.sites._by_id('site-id').lists._by_id('list-id').items._by_id('listItem-id').fields.patch(request_body)


```