---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PrinterShare();
requestBody.setName('name-value');

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.print().shares().post(requestBody);


```