---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintTaskTrigger()
request_body.Event(PrintEvent('jobstarted'))

additionalData = [
'definition@odata.bind' => 'https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}', 
];
request_body.additionaldata(additionalData)





result = await client.print.printers_by_id('printer-id').taskTriggers.post(request_body = request_body)


```