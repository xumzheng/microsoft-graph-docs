---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrinterShare()
request_body.setName('name-value')

additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}', 
];
request_body.setAdditionalData(additionalData)



request_config = SharesRequestBuilderPostRequestConfiguration(
request_config = SharesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.print.shares.post(request_body, headers=)


```