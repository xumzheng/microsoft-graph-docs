---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PrinterShare()
request_body.setDisplayName('ShareName')

request_body.setAllowAllUsers(true)

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}', 
];
request_body.setAdditionalData(additionalData)




result = await client.print.sharesById('printerShare-id').patch(request_body)


```