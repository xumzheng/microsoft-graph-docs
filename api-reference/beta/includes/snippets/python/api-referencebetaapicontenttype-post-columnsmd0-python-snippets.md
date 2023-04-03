---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ColumnDefinition();
additionalData = [
'sourceColumn@odata.bind' => 'https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103', 
];
requestBody.setAdditionalData(additionalData);




result = await client.sitesById('site-id').contentTypesById('contentType-id').columns().post(requestBody);


```