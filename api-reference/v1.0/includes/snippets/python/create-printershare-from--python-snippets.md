---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PrinterShare();
requestBody.setDisplayName('ShareName');

requestBody.setAllowAllUsers(false);

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/v1.0/print/printers/{printerId}', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.print().shares().post(requestBody);


```