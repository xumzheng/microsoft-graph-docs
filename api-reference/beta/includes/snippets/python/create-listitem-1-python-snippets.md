---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ListItem();
fields = FieldValueSet();
additionalData = [
'Title' => 'Widget', 
'Color' => 'Purple', 
'Weight' => 32,
];
fields.setAdditionalData(additionalData);



requestBody.setFields($fields);


result = await client.sitesById('site-id').listsById('list-id').items().post(requestBody);


```