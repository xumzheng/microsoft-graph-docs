---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PrinterShare();
requestBody.setName('name-value');

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.print().shares().post(requestBody);


```