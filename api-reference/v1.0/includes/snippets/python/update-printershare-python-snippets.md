---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrinterShare()
request_body.displayName = 'PrinterShare Name'

request_body.allow_all_users = False

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/v1.0/print/printers/{printerId}', 
];
request_body.additionaldata(additionalData)





result = await client.print.shares_by_id('printerShare-id').patch(request_body = request_body)


```