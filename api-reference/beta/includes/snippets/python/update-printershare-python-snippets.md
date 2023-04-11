---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrinterShare()
request_body.displayName = 'ShareName'

request_body.allowAllUsers = true

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}', 
];
request_body.additionaldata(additionalData)




request_configuration = PrinterShareRequestBuilderPatchRequestConfiguration(
)


result = await client.print.shares_by_id('printerShare-id').patch(request_body = request_body)


```