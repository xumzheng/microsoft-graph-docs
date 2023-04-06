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



request_config = FieldsRequestBuilderPatchRequestConfiguration(
request_config = FieldsRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items_by_id('listItem-id').fields.patch(request_body, headers=)


```