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
fields.additionaldata(additionalData)



request_body.fields = fields


request_configuration = ItemsRequestBuilderPostRequestConfiguration(
)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items.post(request_body = request_body)


```