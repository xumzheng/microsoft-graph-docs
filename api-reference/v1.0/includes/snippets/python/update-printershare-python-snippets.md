---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PrinterShare();
requestBody.setDisplayName('PrinterShare Name');

requestBody.setAllowAllUsers(false);

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/v1.0/print/printers/{printerId}', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.print().sharesById('printerShare-id').patch(requestBody);


```