---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PrinterShare();
requestBody.setDisplayName('ShareName');

requestBody.setAllowAllUsers(true);

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.print().sharesById('printerShare-id').patch(requestBody);


```