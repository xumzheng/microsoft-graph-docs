---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ListItem();
fields = FieldValueSet();
additionalData = [
'Title' => 'Widget', 
'Color' => 'Purple', 
'Weight' => 32,
];
fields.setAdditionalData(additionalData);



requestBody.setFields($fields);


requestResult = graphServiceClient.sitesById('site-id').listsById('list-id').items().post(requestBody);


```