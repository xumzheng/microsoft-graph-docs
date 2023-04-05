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




result = await client.sitesby_id('site-id').listsby_id('list-id').itemsby_id('listItem-id').fields.patch(request_body)


```