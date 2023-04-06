---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ListItem()
fields = FieldValueSet()
additionalData = [
'Title' => 'Widget', 
'Color' => 'Purple', 
'Weight' => 32,
];
fields.setAdditionalData(additionalData)



request_body.setFields($fields)

request_config = ItemsRequestBuilderPostRequestConfiguration(
request_config = ItemsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items.post(request_body, headers=)


```