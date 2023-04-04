---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PrinterShare();
request_body.setDisplayName('ShareName');

request_body.setAllowAllUsers(false);

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/v1.0/print/printers/{printerId}', 
];
request_body.setAdditionalData(additionalData);




result = await client.print().shares().post(request_body);


```