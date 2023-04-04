---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ColumnDefinition()
additionalData = [
'sourceColumn@odata.bind' => 'https://graph.microsoft.com/v1.0/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103', 
];
request_body.setAdditionalData(additionalData)




result = await client.sitesById('site-id').contentTypesById('contentType-id').columns.post(request_body)


```